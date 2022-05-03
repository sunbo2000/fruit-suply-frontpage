<template>
  <el-container>
      <el-header style="height: 110px; margin: 0; padding: 0px; border: 0">
        <el-row>
          <el-col :span="24">
            <div class="top1">
              <div class="slogan">果宝特供，您的云端农场</div>
            </div>
            <div class="square">
              <img class="logoUrl" src="~/assets/img/img.png" alt="logo"/>
              <div class="logoFont">宝特供</div>
              <input class="search" placeholder="来看看吧~"></input>
              <button class="seaSquare">搜索</button>
              <div class="el-icon-user"
                   style=" display: inline-block; position: relative; margin-left: 100px; font-size: 35px;color: rgb(255,255,255); height: 35px;top: -28px;left: 360px;">
              </div>
              <div class="fontLogin">登录</div>
              <div class="el-icon-shopping-cart-2"
                   style="display: inline-block;  position: relative; width: 100px; font-size: 35px;color: rgb(255,255,255); height: 35px;top: -28px;left: 360px;">
              </div>
              <div class="fontShop">购物车</div>
              <div class="el-icon-s-help"
                   style="display: inline-block;  position: relative; width: 100px; font-size: 35px;color: rgb(255,255,255); height: 35px;top: -28px;left: 300px;">
              </div>
              <div class="vip">vip</div>
              <div class="el-icon-question"
                   style="display: inline-block;  position: relative; width: 100px; font-size: 35px;color: rgb(255,255,255); height: 35px;top: -28px;left: 190px;">
              </div>
              <div class="help">帮助</div>
            </div>
          </el-col>
        </el-row>
      </el-header>
    <nuxt/>
  </el-container>
</template>
<style scoped>

.top1 {
  /* 矩形 1 */
  padding: 5px;
  height: 32px;
  text-align: center;
  background: rgb(215, 245, 109);
}

.slogan {
  /* 果宝特供，您的云端农场 */
  text-align: center;
  color: rgb(24, 77, 71);
  font-family: Noto Sans SC, serif;
  font-size: 14px;
  font-weight: 400;
  line-height: 21px;
  letter-spacing: 20px;
}

.square {
  /* 矩形 2 */
  height: 66px;
  top: 32px;
  left: 0;
  background: rgb(24, 77, 71);
}

.logoUrl {
  /* logo */
  width: 45px;
  height: 62px;
  display: inline-block;
}

.logoFont {
  /* 宝特供 */
  position: relative;
  top: -25px;
  display: inline-block;
  width: 164px;
  height: 50px;

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
  display: inline-block;
  position: relative;
  width: 595px;
  height: 26px;
  top: -35px;
  left: 300px;

  background: rgb(255, 255, 255);
}

.seaSquare {
  /* 矩形 4 */
  display: inline-block;
  position: relative;
  width: 55px;
  height: 32px;
  top: -34px;
  left: 290px;
  color: rgb(255, 255, 255);
  cursor: pointer;

  background: rgb(238, 187, 77);
}

.fontLogin {
  /* 登录 */
  display: inline-block;
  position: relative;
  width: 80px;
  height: 21px;
  top: -30px;
  left: 360px;


  color: rgb(255, 255, 255);
  font-family: HappyZcool-2016, '楷体', '楷体_GB2312', serif;
  font-size: 30px;
  font-weight: 400;
  line-height: 21px;
  letter-spacing: 0px;
  text-align: left;

}

.fontShop {
  display: inline-block;
  position: relative;
  width: 100px;
  height: 21px;
  top: -30px;
  left: 300px;


  color: rgb(255, 255, 255);
  font-family: HappyZcool-2016, '楷体', '楷体_GB2312', serif;
  font-size: 30px;
  font-weight: 400;
  line-height: 21px;
  letter-spacing: 0px;
  text-align: left;
}

.vip {
  display: inline-block;
  position: relative;
  width: 100px;
  height: 21px;
  top: -30px;
  left: 240px;


  color: rgb(255, 255, 255);
  font-family: HappyZcool-2016, '楷体', '楷体_GB2312', serif;
  font-size: 30px;
  font-weight: 400;
  line-height: 21px;
  letter-spacing: 0px;
  text-align: left;
}

.help {
  display: inline-block;
  position: relative;
  width: 70px;
  height: 21px;
  top: -30px;
  left: 130px;


  color: rgb(255, 255, 255);
  font-family: HappyZcool-2016, '楷体', '楷体_GB2312', serif;
  font-size: 30px;
  font-weight: 400;
  line-height: 21px;
  letter-spacing: 0px;
  text-align: left;
}

</style>
