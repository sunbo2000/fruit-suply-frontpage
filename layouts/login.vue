<template>
  <el-container class="all">
    <el-header class="pbmHeader">
      <div class="top1">
        <div class="slogan">果宝特供，您的云端农场</div>
      </div>
      <div class="square">
      </div>
      <img class="logoUrl" src="~/assets/img/img.png" alt="logo"/>
      <div class="logoFont">宝特供</div>
<!--      <input class="search" placeholder="来看看吧~"></input>-->
<!--      <el-button size="mini" class="seaSquare">搜索</el-button>-->

      <!--      <img class="square4" src="~/assets/img/img_1.png" alt="banner"/>-->
      <!--      <img class="square5" src="~/assets/img/img_2.png" alt="logo">-->
      <!--      <div class="des">果宝特供</div>-->
    </el-header>
      <nuxt/>

  </el-container>
</template>
<style scoped>
.all {
  width: 1920px;
  overflow: hidden;
  margin: -10px;
  padding: 0;
  border: 0;
}

.pbmHeader {
  position: relative;
  height: 100px !important;
  margin: 0;
  padding: 0;
  border: 0;
}

.top1 {
  /* 矩形 1 */
  position: absolute;
  width: 100%;
  height: 32px;
  top: 0;
  left: 0;
  background: rgb(215, 245, 109);
}

.slogan {
  /* 果宝特供，您的云端农场 */
  position: absolute;
  width: 430px;
  height: 21px;
  top: 5px;
  left: 783px;


  color: rgb(24, 77, 71);
  font-family: "MS UI Gothic", sans-serif;
  font-size: 14px;
  font-weight: 400;
  line-height: 21px;
  letter-spacing: 20px;
}

.square {

  /* 矩形 2 */
  position: absolute;
  width: 100%;
  height: 66px;
  top: 32px;
  left: 0;


  background: rgb(24, 77, 71);
  /* 矩形 2 */
}

.logoUrl {
  /* logo */
  position: absolute;
  width: 45px;
  height: 59px;
  top: 43px;
  left: 8px;

}

.logoFont {

  /* 宝特供 */
  position: absolute;
  width: 164px;
  height: 50px;
  top: 48px;
  left: 55px;


  color: rgb(255, 255, 255);
  font-family: HappyZcool-2016, serif;
  font-size: 36px;
  font-weight: 400;
  line-height: 41px;
  letter-spacing: 0px;
  text-align: left;


}

a {
  color:  #184d47;
  text-decoration: none;
}

a:hover {
  color: cornflowerblue;
}


</style>
