<template>
  <el-container class="all">
    <el-header class="pbmHeader">
      <div class="top1">
        <div class="slogan">果宝特供，您的云端农场</div>
      </div>
      <div class="square"><img class="userLogo" src="~/assets/img1/user.png" alt=""/><span class="MyFarm">我的智慧农场</span>
      </div>
      <img class="logoUrl" src="~/assets/img/img.png" alt="logo"/>
      <div class="logoFont">宝特供</div>
      <input class="search" placeholder="来看看吧~"></input>
      <el-button size="mini" class="seaSquare">搜索</el-button>

<!--      <img class="square4" src="~/assets/img/img_1.png" alt="banner"/>-->
<!--      <img class="square5" src="~/assets/img/img_2.png" alt="logo">-->
<!--      <div class="des">果宝特供</div>-->
    </el-header>
    <el-container>
      <el-aside class="pbmAside">
        <div class="block">
          <div class="container1">
            <div class="buttonBgWrapper">
              <img class="buttonBg1" src="~/assets/img1/img_11.png"/>
              <p class="title3">智慧农业检测平台</p>
            </div>
            <div class="actionBgWrapperItem0">
              <a href="/admin">
                <img class="actionBg2" src="~/assets/img1/img_13.png"/>
                <span class="caption3">农场管理</span></a>
            </div>
            <a href="#">
              <div class="actionBgWrapperItem0">
                <img class="buttonBg2" src="~/assets/img1/img_13.png"/>
                <span class="caption04">系统分析</span>
              </div>
            </a>

            <div class="actionBgWrapperItem0">
              <a href="/admin">
                <img class="actionBg3" src="~/assets/img1/img_13.png"/>
                <span class="caption5">数据采集</span></a>
            </div>
            <div class="actionBgWrapperItem0">
              <a href="/admin">
                <img class="buttonBg3" src="~/assets/img1/img_13.png"/>
                <span class="caption6">视频教学</span></a>
            </div>
            <div class="actionBgWrapperItem0">
              <a href="/admin">
                <img class="actionBg4" src="~/assets/img1/img_13.png"/>
                <span class="caption7">问题反馈</span></a>
            </div>
            <div class="actionBgWrapperItem0">
              <a href="/admin">
                <img
                  class="buttonBg4"
                  src="~/assets/img1/img_13.png"
                />
                <span class="caption8">系统搭建</span></a>
            </div>
            <div class="actionBgWrapperItem0">
              <a href="/admin">
                <img
                  class="actionBg5"
                  src="~/assets/img1/img_13.png"
                />
                <span class="caption9">消费趋势</span></a>
            </div>
          </div>
          <img
            class="layer"
            src="~/assets/img1/img_19.png"
          />
        </div>
      </el-aside>
      <nuxt/>
    </el-container>
    <el-footer class="pbmFooter">
      <div class="footer2">
        <div class="footer4">
          <div class="footer5"><span class="fontFooter">鲜</span></div>
          <div class="footer5"><span class="fontFooter">快</span></div>
          <div class="footer5"><span class="fontFooter">绿</span></div>
          <div class="footer5"><span class="fontFooter">质</span></div>
          <div class="footer6"><span class="fontFooter">免</span></div>
        </div>
        <div class="logo1">
          <svg-icon class="logo2" style="font-size: 290px" icon-class="footerLogo"/>
          <p class="logoFont3">果宝特供</p>
        </div>
        <div class="footer01">
          <span class="footer01-foot">物鲜味美</span>
          <span class="footer01-foot">送货快速</span>
          <span class="footer01-foot">科学种植</span>
          <span class="footer01-foot">质量最佳</span>
          <span class="footer01-foot1">免费咨询</span>
        </div>
        <div class="footer02">
          <span class="footer02-foot"></span>
          <span class="footer02-foot"></span>
          <span class="footer02-foot"></span>
          <span class="footer02-foot"></span>
          <span class="footer02-foot1"></span>
        </div>
        <div class="footer03">
          <span class="footer03-foot">我们保证提供给您的鲜果是最新鲜、口感最好的</span>
          <span class="footer03-foot">我们会以最快速度发货，且我们支持同城配送</span>
          <span class="footer03-foot">产品采用科学种植方式，不添加任何有害物质</span>
          <span class="footer03-foot">如果您对我们的产品不满意，可申请退款</span>
          <span class="footer03-foot1">如果您对产品有疑问，可免费咨询我们的客服</span>
        </div>
      </div>
      <div class="footer3"><span class="footer9">果宝特供，您的云端农场</span></div>
    </el-footer>

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

.pbmAside {
  position: relative;
  width: 460px !important;
  margin: 0;
  padding: 0;
  border: 0;

}

.pbmFooter {
  position: relative;
  height: 609px !important;
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
  width: 400px;
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

.search {
  /* 矩形 3 */
  position: absolute;
  width: 580px;
  height: 26px;
  top: 49px;
  border-radius: 4px;
  left: 660px;
  font-size: 15px;
  padding-left: 10px;
  padding-right: 10px;


  background: rgb(255, 255, 255);
}

.seaSquare {
  /* 矩形 4 */
  position: absolute;
  width: 57px;
  height: 30px;
  top: 50px;
  left: 1270px;
  padding: 2px;
  color: rgb(255, 255, 255);
  cursor: pointer;
  font-size: 15px;

  background: rgb(238, 187, 77);
}

.userLogo {
  /* circle-user */
  position: absolute;
  width: 35px;
  height: 35px;
  top: 17px;
  left: 1735px;
}

.square4 {
  /* pexels-trang-doan-1128678 1 */
  position: absolute;
  width: 100%;
  height: 719px;
  top: 98px;
  left: 0;
}

.square5 {
  /* logo无字 1 */
  position: absolute;
  width: 560px;
  height: 494px;
  top: 164px;
  left: -12px;

}

.des {
  /* 果宝特供 */
  position: absolute;
  width: 415px;
  height: 128px;
  top: 629px;
  left: 61px;


  color: rgb(24, 77, 71);
  font-family: 黑体, HappyZcool-2016, serif;
  font-size: 100px;
  font-weight: 400;
  line-height: 114px;
  letter-spacing: 0px;
  text-align: left;

}

.footer2 {
  /* 矩形 3 */
  position: relative;
  height: 577px;
  top: 0;
  left: 0;
  background: rgb(24, 77, 71);
}


.footer4 {
  /* 鲜快绿质免 */
  position: absolute;
  width: 1344px;
  height: 120px;
  top: 112px;
  left: 88px;
}

.footer5 {
  /* 矩形 4 */
  display: inline-block;
  position: relative;
  width: 120px;
  height: 120px;
  margin-right: 181px;
  text-align: center;

  background: rgba(215, 245, 109, 0.05);
}

.footer6 {
  /* 矩形 4 */
  display: inline-block;
  position: relative;
  width: 120px;
  height: 120px;
  text-align: center;

  background: rgba(215, 245, 109, 0.05);
}

.fontFooter {
  /* 鲜 */
  position: relative;
  top: 5px;
  width: 89px;


  color: rgba(246, 190, 80, 0.45);
  font-family: "Microsoft JhengHei UI", HappyZcool-2016, serif;
  font-size: 88px;
  font-weight: 400;
  line-height: 100px;
  letter-spacing: 0px;
  text-align: center;
}

.logo1 {
  /* logo */
  position: absolute;
  width: 365px;
  height: 448px;
  top: 81px;
  left: 1528px;
  text-align: center;
}

.logo2 {
  /* 矩形 2 */
  position: absolute;
  left: -2px;
}

.logoFont3 {
  /* 果宝特供 */
  position: relative;
  top: 250px;


  color: rgba(246, 190, 80, 0.53);
  font-size: 70px;
  font-weight: 400;
  line-height: 80px;
  letter-spacing: 0px;
  font-family: "MS UI Gothic", HappyZcool-2016, serif;

}

.footer01 {
  /* 文字 二级 */
  position: absolute;
  width: 1367px;
  height: 40px;
  top: 277px;
  left: 81px;


}

.footer01-foot {
  /* 物鲜味美 */
  display: inline-block;
  position: relative;
  width: 141px;
  height: 40px;
  margin-right: 160px;


  color: rgba(246, 190, 80, 0.53);
  font-family: HappyZcool-2016;
  font-size: 35px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0px;
  text-align: left;
}

.footer01-foot1 {
  /* 物鲜味美 */
  display: inline-block;
  position: relative;
  width: 141px;
  height: 40px;


  color: rgba(246, 190, 80, 0.53);
  font-family: HappyZcool-2016;
  font-size: 35px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0px;
  text-align: left;
}

.footer02 {
  position: absolute;
  width: 1402px;
  height: 40px;
  top: 336px;
  left: 65px;
}

.footer02-foot {
  height: 1px;
  border-top: 2px solid rgba(215, 245, 109, 0.7);
  text-align: center;

  /* 物鲜味美 */
  display: inline-block;
  position: relative;
  width: 171px;
  margin-right: 130px;
}

.footer02-foot1 {
  height: 1px;
  border-top: 2px solid rgba(215, 245, 109, 0.7);
  text-align: center;

  /* 物鲜味美 */
  display: inline-block;
  position: relative;
  width: 171px;
}

.footer03 {
  position: absolute;
  width: 1410px;
  height: 120px;
  top: 377px;
  left: 62px;

}

.footer03-foot {
  /* 物鲜味美 */
  display: inline-block;
  position: relative;
  width: 180px;

  margin-right: 121px;

  /* 我们保证提供给 您的鲜果是最新 鲜、口感最好的 */
  height: 120px;


  color: rgba(246, 190, 80, 0.53);
  font-family: HappyZcool-2016;
  font-size: 25px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0px;

}

.footer03-foot1 {
  /* 物鲜味美 */
  display: inline-block;
  position: relative;
  width: 180px;

  /* 我们保证提供给 您的鲜果是最新 鲜、口感最好的 */
  height: 120px;


  color: rgba(246, 190, 80, 0.53);
  font-family: HappyZcool-2016;
  font-size: 25px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0px;

}

.footer3 {
  /* 矩形 1 */
  position: relative;
  height: 32px;
  background: rgb(215, 245, 109);
  text-align: center;
  padding-top: 4px;
}

.footer9 {
  /* 果宝特供，您的云端农场 */
  color: rgb(24, 77, 71);
  font-family: Noto Sans SC;
  font-size: 14px;
  font-weight: 400;
  line-height: 21px;
  letter-spacing: 20px;
  text-align: left;

}

.MyFarm {
  /* 我的智慧农场 */
  position: absolute;
  width: 108px;
  height: 21px;
  top: 22px;
  left: 1780px;


  color: rgb(255, 255, 255);
  font-family: 幼圆, HappyZcool-2016, serif;
  font-size: 18px;
  font-weight: 500;
  line-height: 21px;
  letter-spacing: 0px;
  text-align: left;


}

.block {
  position: relative;
  width: 300px;
  top: 75px;
  left: 160px;

}

.container1 {
  position: relative;
  background-image: url("~/assets/img1/img_32.png");
  width: 300px;
  height: 754px;
}

.buttonBgWrapper {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: row;
  justify-content: center;
  width: 300px;
  height: 118px;
}

.buttonBg1 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 105px;
}

.title3 {
  position: relative;
  margin-top: 10px;
  letter-spacing: 2px;
  line-height: 40px;
  color: #ffffff;
  font-size: 35px;
  font-weight: 400;
  width: 150px;
  height: 90px;
}


.actionBgWrapperItem0 {
  display: flex;
  position: relative;
  margin-top: 20px;
  align-items: center;
  flex-direction: row;
  width: 300px;
  height: 71px;
  cursor: pointer;
}

.actionBgWrapperItem01 {
  display: flex;
  position: absolute;
  background-color: black;
  top: 106px;
  left: 910px;
}

.actionBg2 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.caption3 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  text-overflow: ellipsis;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  font-size: 40px;
  font-weight: 400;
}


.buttonBg2 {
  position: absolute;
  left: 0px;
  width: 300px;
  height: 71px;
}

.caption04 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  text-overflow: ellipsis;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  font-size: 40px;
  font-weight: 400;
  color: #9c4e04;
}

.actionBg3 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.caption5 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  overflow: hidden;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  font-size: 40px;
  font-weight: 400;
}

.buttonBg3 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.caption6 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  overflow: hidden;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  font-size: 40px;
  font-weight: 400;
}

.actionBg4 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.caption7 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  overflow: hidden;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  font-size: 40px;
  font-weight: 400;
}

.buttonBg4 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.caption8 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  overflow: hidden;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  font-size: 40px;
  font-weight: 400;
}

.title9 {
  position: absolute;
  top: 545px;
  left: 48px;
  line-height: 60px;
  letter-spacing: 15px;
  white-space: nowrap;
  font-size: 40px;
  font-weight: 400;
}

.actionBgWrapperItem5 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  margin-top: 19px;
  width: 300px;
  height: 71px;
}

.actionBg5 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.caption9 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  overflow: hidden;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  font-size: 40px;
  font-weight: 400;
}

.title10 {
  position: absolute;
  bottom: 58px;
  left: 48px;
  line-height: 60px;
  letter-spacing: 15px;
  white-space: nowrap;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
}

.caption10 {
  position: absolute;
  top: 727px;
  left: 48px;
  line-height: 60px;
  letter-spacing: 15px;
  white-space: nowrap;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
}

.layer {
  position: relative;
  margin-top: 40px;
  width: 300px;
  height: 1028px;
}

a {
  color:  #184d47;
  text-decoration: none;
}

a:hover {
  color: cornflowerblue;
}
</style>
