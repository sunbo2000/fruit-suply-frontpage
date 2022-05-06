<template>
  <div class="all">
    <header class="pbmHeader">
      <div class="top1">
        <div class="slogan">果宝特供，您的云端农场</div>
      </div>
      <div class="square"></div>
      <img class="logoUrl" src="~/assets/img/img.png" alt="logo"/>
      <div class="logoFont">宝特供</div>
      <input class="search" placeholder="来看看吧~"></input>
      <el-button size="mini" class="seaSquare">搜索</el-button>

      <a v-if="user === ''" href="/login">
        <div class="loginLogo">
          <span class="el-icon-user-solid"></span>
        </div>
        <div class="fontLogin">登录</div>
      </a>
      <a href="#">
      <img class="avatar1" :src="user.avatar" alt="avatar"/></a>

      <a href="#">
        <div class="shopLogo"
        ><span class="el-icon-shopping-cart-2"></span>
        </div>
        <div class="fontShop">购物车</div>
      </a>

      <a href="#">
        <div class="vipLogo">
          <span class="el-icon-s-help"></span>
        </div>
        <div class="vip">vip</div>
      </a>

      <a href="#">
        <div class="helpLogo">
          <span class="el-icon-question"></span>
        </div>
        <div class="help">帮助</div>
      </a>
      <img class="square4" src="~/assets/img/img_1.png" alt="banner"/>
      <img class="square5" src="~/assets/img/img_2.png" alt="logo">
      <div class="des">果宝特供</div>
    </header>
    <nuxt/>
    <footer class="pbmFooter">
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
    </footer>
  </div>
</template>
<script>
import cookie from "js-cookie";

export default {
  data() {
    return {
      //  数据
      user: ''
    }
  },
  created() {
    let identity = cookie.get("user");
    if (identity) {
      this.user = {
        name: identity,
        avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
      }
      console.log(this.user)
    }
  },

  methods: {
    //  编写方法
  }
}

</script>
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
  height: 818px;
}

.pbmFooter {
  position: relative;
  height: 609px;
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

.loginLogo {
  /* circle-user */
  position: absolute;
  width: 35px;
  height: 35px;
  top: 47px;
  left: 1555px;
  z-index: 1;

  font-size: 30px;
  color: rgb(255, 255, 255);
}

.fontLogin {
  /* 登录 */
  position: absolute;
  width: 100px;
  height: 21px;
  top: 57px;
  left: 1590px;


  color: rgb(255, 255, 255);
  font-family: 黑体, serif;
  font-size: 20px;
  font-weight: 400;
  line-height: 21px;
  letter-spacing: 0px;
  text-align: left;

}

.shopLogo {
  /* shopping-cart-2-fill */
  position: absolute;
  width: 35px;
  height: 35px;
  top: 47px;
  left: 1635px;

  font-size: 30px;
  color: rgb(255, 255, 255);
}

.fontShop {
  /* 购物车 */
  position: absolute;
  width: 70px;
  height: 21px;
  top: 57px;
  left: 1670px;


  color: rgb(255, 255, 255);
  font-family: 黑体, HappyZcool-2016, serif;
  font-size: 20px;
  font-weight: 400;
  line-height: 21px;
  letter-spacing: 0px;
  text-align: left;
}

.vipLogo {
  /* vip-fill */
  position: absolute;
  width: 35px;
  height: 35px;
  top: 47px;
  left: 1740px;

  font-size: 30px;
  color: rgb(255, 255, 255);
}

.vip {
  /* VIP */
  position: absolute;
  width: 29px;
  height: 21px;
  top: 57px;
  left: 1775px;


  color: rgb(255, 255, 255);
  font-family: 黑体, HappyZcool-2016, serif;
  font-size: 20px;
  font-weight: 400;;
  line-height: 21px;
  letter-spacing: 0px;
  text-align: left;


}

.helpLogo {
  /* Help */
  position: absolute;
  width: 35px;
  height: 35px;
  top: 47px;
  left: 1815px;

  font-size: 30px;
  color: rgb(255, 255, 255);

}

.help {
  /* 帮助 */
  position: absolute;
  width: 50px;
  height: 21px;
  top: 57px;
  left: 1850px;


  color: rgb(255, 255, 255);
  font-family: 黑体, HappyZcool-2016, serif;
  font-size: 20px;
  font-weight: 400;
  line-height: 21px;
  letter-spacing: 0px;
  text-align: left;


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
.avatar1{
  /* circle-user */
  position: absolute;
  width: 40px;
  height: 40px;
  top: 47px;
  left: 1575px;
  z-index: 1;
  border-radius: 50%;
  font-size: 30px;
  color: rgb(255, 255, 255);
}
</style>
