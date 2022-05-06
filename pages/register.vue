<template>
  <el-main class="pbmMain">
    <div class="div2">
      <div class="div1">
        <div style="text-align: center; margin-bottom: 20px">
          <a href="/login">登录账号</a>&nbsp;
          <a href="#" style="color: lightseagreen">注册账号</a>
        </div>

        <el-form
          ref="userForm"
          :model="params"
          :hide-required-asterisk="true"
          label-position="top"
        >
          <el-form-item class="item" label="身份" prop="identity">
            <el-select class="input2" style="" v-model="params.identity" placeholder="请选择要注册的身份">
              <el-option label="用户" value="1"></el-option>
              <el-option label="商家" value="2"></el-option>
            </el-select>
          </el-form-item>
          <el-form-item
            class="item"
            label="用户名"
            prop="nickname"
            :rules="[
            {
              required: true,
              message: '请输入用户名',
              trigger: 'blur',
            },
            {
              required: true,
              pattern: /^(?!_)(?!.*?_$)[a-zA-Z0-9_\u4e00-\u9fa5]+$/,
              message: '名称只能包含汉字,数字,字母,_,不能以_开头或结尾',
              trigger: 'blur',
            },
            { min: 4, max: 12, message: '长度不能超过12位', trigger: 'blur' }
          ]"
          >
            <el-input
              type="text"
              placeholder="汉字,字母,数字,_组成,不能以_开头或结尾,最多12位"
              v-model="params.nickname"
            />
          </el-form-item>
          <el-form-item
            class="item"
            label="设置密码"
            prop="password"
            :rules="[{ required: true, message: '请输入密码', trigger: 'blur' },
          { min: 6, message: '密码至少6位', trigger: 'blur' },
          { max: 16, message: '密码最多16位', trigger: 'blur' }]"
          >
            <el-input
              type="password"
              placeholder="设置6~16位密码"
              v-model="params.password"
            />
          </el-form-item>
          <el-form-item
            class="item"
            label="确认密码"
            prop="checkPass"
            :rules="[
            { required: true, message: '请再次输入密码', trigger: 'blur' },
            { validator: checkPassword, trigger: 'blur' },
          ]"
          >
            <el-input
              type="password"
              placeholder="确认密码"
              v-model="params.checkPass"
            />
          </el-form-item>
          <el-form-item
            class="item"
            label="手机号码"
            prop="mobile"
            :rules="[
            { required: true, message: '请输入手机号码', trigger: 'blur' },
            { validator: checkPhone, trigger: 'blur' },
          ]"
          >
            <el-input
              type="text"
              placeholder="填写你常用的手机号码作为登录账号"
              v-model="params.mobile"
            />
          </el-form-item>

          <el-form-item
            class="item"
            label="短信验证码"
            prop="code"
            :rules="[
            { required: true, message: '请输入验证码', trigger: 'blur' },
          ]"
          >
            <el-input
              type="text"
              placeholder="填写短信验证码"
              v-model="params.code"
              class="input1"
            />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            <el-button
              type="info"
              :plain="true"
              :value="codeTest"
              @click="getCodeFun()"
            >
              {{ codeTest }}
            </el-button>
          </el-form-item>

          <div style="text-align: center; margin-top: 30px">
            <el-button
              style="width: 2.61rem; height: 35px; font-size: 19px"
              type="success"
              class="sign-up-button"
              @click="submitForm('userForm')"
            >注 册</el-button>
          </div>
          <p  style="position: relative; top: 10px">
            点击"注册"即表示您同意并愿意遵守果宝特供用户协议和隐私政策
          </p>
        </el-form>
      </div>
    </div>
  </el-main>
</template>
<script>

export default {
  layout: "login",
  data() {
    return {
      params: {
        identity: '',
        mobile: "",
        code: "",
        nickname: "",
        password: "",
        checkPass: "",
      },
      sending: true, //是否发送验证码
      second: 120, //倒计时间
      codeTest: "获取短信验证码",
    };
  },
  methods: {
    //
    submitForm(formName) {
      this.$refs[formName].validate((valid) => {
        if (valid) {
          window.location.href="/login"
        } else {
          console.log('error submit!!');
          return false;
        }
      });
    },
    qqRegister() {
      this.$message.warning("开发中,敬请期待......");
    },
    getCodeFun() {
      //sending = false
      //this.sending原为true,请求成功，!this.sending == true，主要是防止有人把disabled属性去掉，多次点击；
      if (!this.sending) return;
      //debugger
      // prop 换成你想监听的prop字段
      this.$refs.userForm.validateField("mobile", (errMsg) => {
        if (errMsg == "") {
          register.sendMessage(this.params.mobile).then((res) => {
            this.sending = false;
            this.timeDown();
          });
        }
      });
    },
    //提交注册表单
    submitRegister() {
      register.register(this.params).then((response) => {
        if (response.data.success) {
          this.$message.success("注册成功");
          this.$router.push({path: "/login"});
        } else {
          this.$message.error(response.data.message);
        }
      });
    },
    //倒计时
    timeDown() {
      this.codeTest = this.second + " 秒后重新获取";
      let result = setInterval(() => {
        this.second--;
        this.codeTest = this.second + " 秒后重新获取";
        if (this.second < 1) {
          clearInterval(result);
          this.sending = true;
          //this.disabled = false;
          this.second = 120;
          this.codeTest = "获取验证码";
        }
      }, 1000);
    },
    checkPhone(rule, value, callback) {
      //debugger
      if (!/^1[34578]\d{9}$/.test(value)) {
        return callback(new Error("手机号码格式不正确"));
      }
      return callback();
    },
    //二次密码输入
    checkPassword(rule, value, callback) {
      if (value !== this.params.password) {
        callback(new Error("两次输入密码不一致!"));
      } else {
        callback();
      }
    },
  },
};
</script>
<!--
	.item: 是绑定class的
	.el-form-item__label: 自动匹配form表单中label的(注意:中间是连续的两个'_')
-->
<style scoped>

.div2 {
  margin: 0;
  padding: 0;
  height: 900px;
  background-color: rgb(250, 250, 250);
}

.div1 {
  position: absolute;
  border-radius: 4%;
  left: 650px;
  top: 110px;
  width: 500px;
  height: 790px;
  padding: 50px;
  background-color: rgb(255, 255, 255);

}

.pbmMain {
  margin: 0;
  padding: 0;
  border: 0;
}
.item /deep/ .el-form-item__error{
  color: indianred;
}
.item /deep/ .el-form-item__label {
  margin-bottom: -10px;
  font-size: 20px;
  font-weight: bolder;
}
.item /deep/ .el-form-item{
  margin-top: 5px;
}
a {
  font-size: 25px;
  color: rgb(150, 150, 150);
  text-decoration: none;
}

a:hover {
  color: lightseagreen;

}

/deep/ .el-input__inner{
  height: 45px;
  width: 500px;
  font-size: 20px;
}
.input1{
  width: 300px;
}
.input1 /deep/ .el-input__inner{
  width: 300px;
  height: 45px;
}
.input2 /deep/ .el-input__inner {
  width: 300px
}
</style>
