<template>
  <div style="width: 100%">
    <div class="top">
      <p class="fontP">乒乒乓乓和敌人较量,果宝特供你不可想象</p></div>
    <div class="search">
      <img
        style="position: relative; top: 5px; left: 10px"
        src="~/assets/img/fruitlogo.png"
        width="160px"
        height="50px"
        alt="果宝特供"
      />
      <el-input style="position: relative;top: -12px; left: 280px; width: 550px;" v-model="queryVo.name"
                placeholder="来找找看吧~"></el-input>
      <el-button style="position: relative;top: -12px;  left: 280px; background-color: rgb(249,202,6)" type="primary">
        搜索
      </el-button>
      <div style="display: inline-block; position: relative;width: 300px; height: 50px;   left: 350px;">
        <span style="margin-right: 40px; cursor: pointer">
          <div
            style="display: inline-block; position: relative; top: 3px;  width: 40px; height: 40px; border-radius: 50px;background-color: aliceblue"></div>
          <p style="display: inline-block; position: relative; top: -8px;  color: aliceblue; font-size: 25px;">登录</p>
        </span>

        <span style="cursor: pointer">
          <div
            style="display: inline-block; position: relative; top: 0px;  width: 35px; height: 35px; border-radius: 10px;background-color: aliceblue"></div>
          <p style="display: inline-block; position: relative; top: -8px;  color: aliceblue; font-size: 25px;">购物车</p>
        </span>
      </div>
    </div>
    <nuxt/>
  </div>
</template>
<script>
export default {
  data() {
    return {
      //  数据
      queryVo: {
        name: ''
      }
    }
  },
  created() {
  },
  methods: {
    //  编写方法
  }
}

</script>
<style scoped>
/*css 代码*/
.fontP {
  font-size: 30px;
  font-family: '楷体', '楷体_GB2312', serif;
  margin: auto;
  position: relative;
  top: 10px;
}

.top {
  height: 50px;
  margin-left: -10px;
  margin-right: -10px;
  margin-top: -8px;
  background-color: rgb(159, 223, 42);
  text-align: center;
  color: rgb(250, 250, 250);
}

.search {

  margin-left: -10px;
  margin-right: -10px;
  margin-top: 0px;
  background-color: rgb(48, 66, 16);
}
</style>
