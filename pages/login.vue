<template>
  <el-main class="pbmMain">
    <div class="div2">
      <div class="div1">
        <div style="text-align: center; margin-bottom: 20px">
          <a href="#" style="color: lightseagreen">登录账号</a>&nbsp;
          <a href="/register">注册账号</a>
        </div>
        <div>
          <el-form ref="userForm" :model="user" :hide-required-asterisk="true" label-position="top">
            <el-form-item class="item" label="身份" prop="identity">
              <el-select class="input2" style="" v-model="user.identity" placeholder="活动区域">
                <el-option label="用户" value="1"></el-option>
                <el-option label="商家" value="2"></el-option>
                <el-option label="政府工作人员" value="3"></el-option>
                <el-option label="科技工作者" value="4"></el-option>
              </el-select>
            </el-form-item>
            <el-form-item class="item" label="用户名" prop="mobile" :rules="[
              {required: true, message: '请输入用户名',     trigger: 'blur'},
              { validator: checkPhone, trigger: 'blur' },
              {min: 4,max: 12,message: '用户名格式不正确,4~12位'}
            ]">
              <el-input class="input1" type="text" placeholder="用户名" v-model="user.mobile"/>
            </el-form-item>
            <el-form-item class="item" label="密码" prop="password" :rules="[
              { required: true, message: '请输入密码', trigger: 'blur' },
              { min: 6, message: '密码至少 6 位', trigger: 'blur' },
              { max: 16, message: '密码最多 16 位', trigger: 'blur' },
            ]">
              <el-input class="input1" type="password" placeholder="密码" v-model="user.password"/>
            </el-form-item>
            <div style="text-align: center; margin-top: 30px">
              <el-button type="success" style="width: 2.61rem; height: 40px; font-size: 20px"
                         @click="submitForm('userForm')">登 录
              </el-button>
            </div>
          </el-form>
          <!-- 更多登录方式 -->
        </div>
      </div>
    </div>
  </el-main>
</template>
<script>
import cookie from "js-cookie";

export default {
  layout: "login",
  data() {
    return {
      user: {
        identity: '1',
        mobile: "",
        password: "",
      },
      loginInfo: {},
    };
  },
  methods: {
    //
    submitForm(formName) {
      this.$refs[formName].validate((valid) => {
        if (valid) {
          if (this.user.identity === '1') {
            cookie.set("user", "consumer", {domain: "localhost"});
            window.location.href = "/consumer"
          } else if (this.user.identity === '2') {
            cookie.set("user", "seller", {domain: "localhost"});
            window.location.href = "/seller"
          } else if (this.user.identity === '3') {
            cookie.set("user", "government", {domain: "localhost"});
            window.location.href = "/government"

          } else if (this.user.identity === '4') {
            cookie.set("user", "admin", {domain: "localhost"});
            window.location.href = "/admin"
          }
        } else {
          console.log("error submit!!");
          return false;
        }
      });
    },
    qqLogin() {
      this.$message.warning("开发中,敬请期待...");
    },
    //1.调用登录方法,进行登录,得到返回的token字符串
    submitLogin() {
      login.loginCheck(this.user).then((response) => {
        if (response.data.success) {
          //2.将获取的token字符串放进cookie里面
          //cookie名称, cookie值,作用范围
          cookie.set("mogu_token", response.data.data.token, {
            domain: "localhost",
          });
          //3.请求发送之前被拦截,在请求头里加入token信息
          //4.调用token获取用户信息,为了首页显示
          login.getLoginUserInfo().then((response) => {
            this.loginInfo = response.data.data.loginInfo;
            //这里要将json对象转换成json字符串
            cookie.set("mogu_ucenter", JSON.stringify(this.loginInfo), {
              domain: "localhost",
            });
            window.location.href = "/";
          });
        } else {
          this.$message.error(response.data.message);
        }
      });
    },
    //检查号码格式
    checkPhone(rule, value, callback) {
      //debugger
      if (!/^(?!_)(?!.*?_$)[a-zA-Z0-9_\u4e00-\u9fa5]+$/.test(value)) {
        return callback(new Error("用户名只能包含汉字,数字,字母,_,不能以_开头或结尾"));
      }
      return callback();
    },
  },
};
</script>
<!--
	.item: 是绑定class的
	.el-form-item__label: 自动匹配form表单中label的(注意:中间是连续的两个'_')
-->
<style scoped>
.pbmMain {
  margin: 0;
  padding: 0;
  border: 0;
}

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
  height: 500px;
  padding: 50px;
  background-color: rgb(255, 255, 255);

}

.item /deep/ .el-form-item__error {
  color: indianred;
}


.item /deep/ .el-form-item__label {
  margin-bottom: -10px;
  font-size: 20px;
  font-weight: bolder;
}

.item /deep/ .el-form-item {
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

/deep/ .el-input__inner {
  height: 45px;
  width: 500px;
  font-size: 20px;
}

.input2 /deep/ .el-input__inner {
  width: 300px
}
</style>
