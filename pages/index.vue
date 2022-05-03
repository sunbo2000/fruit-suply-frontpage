<template>
  <!--  在这里写html,vue前端代码-->
  <el-main style="margin: 0; padding: 0; border: 0">
    <div class="web1">
      <img class="square4" src="~/assets/img/img_1.png" alt="banner"/>
      <img class="square5" src="~/assets/img/img_2.png" alt="logo">
      <div class="des">果宝特供</div>
    </div>
  </el-main>
</template>

<script>
export default {
  data() {
    return {
      //  数据
    }
  },

  methods: {
    //  编写方法
  }
}

</script>
<style scoped>
/*css 代码*/
.web1 {
  position: relative;
  width: 100%;
  height: 800px;
  left: 0;

  background: rgb(255, 255, 255);
}

.square4 {
  position: absolute;
  width: 100%;
  left: 0;
}

.square5 {
  /* logo无字 1 */
  position: relative;
  width: 560px;
  height: 494px;
  top: 0px;
  left: -12px;
}

.des {
  /* 果宝特供 */
  position: relative;
  width: 415px;
  height: 128px;
  top: 0px;
  left: 61px;


  color: rgb(24, 77, 71);
  font-family: HappyZcool-2016, serif;
  font-size: 100px;
  font-weight: 400;
  line-height: 114px;
  letter-spacing: 0px;
  text-align: left;


}
</style>
