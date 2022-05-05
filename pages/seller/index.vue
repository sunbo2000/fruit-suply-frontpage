<template>
  <!--  卖家页面-->
  <!--  在这里写html,vue前端代码-->
  <main class="main">
  <div class="seller">
    <div class="supply">
      <div class="tag_supply">
        <svg-icon style="font-size: 200px; position: absolute; top: -50px; left: 10px;" icon-class="supply"/>
      </div>
      <div class="body"
           style="position: absolute;height: 400px;width: 500px;top:100px;left: 20px;">
        <div class="block1"
          style="position:absolute;height: 400px;width: 500px;top: 0;left: 0;">
          <img
            src="~/assets/img/img_170.png"
            style="position: absolute;height: 400px;width: 500px;top: 0;left: 0;">
          <p
            style="position: absolute;left:10px;color: rgb(255, 255, 255);font-family: HappyZcool-2016,sans-serif;font-size: 120px;font-weight: 400;line-height: 137px;letter-spacing: 0px;text-align: center;">
            农用机械</p>
        </div>
        <div class="block2"
          style="position: absolute;left:530px;top:0;height: 400px;width:300px;">
          <div style="position: absolute;top:0;left:0;height: 180px;width:300px;text-align:center;">
            <img
              style="position: relative;top:0px;left:0px;height: 180px;width:300px;"
              src="~/assets/img/img_171.png">
            <p
              style=" position:absolute;top:-10px;left:30px;color: rgb(255, 255, 255);font-family:sans-serif;font-size: 60px;font-weight: 400;line-height: 91px;letter-spacing: 0;">
              种子种苗
            </p>
          </div>
          <div style="position: absolute;bottom:0px;left:0px;height: 180px;width:300px;text-align: center;">
            <img
              style="position: absolute;position: relative;bottom:0px;left:0px;height: 180px;width:300px;"
              src="~/assets/img/img_172.png">
            <p
              style=" position:absolute;top:-10px;left:30px;color: rgb(255, 255, 255);font-family:sans-serif;font-size: 60px;font-weight: 400;line-height: 91px;letter-spacing: 0;">
              动物饲料
            </p>
          </div>
        </div>
        <div class="block3"
          style="left:860px;position: absolute;top:0;height: 400px;width:180px;">
          <div style="top:0;position: absolute;height: 180px;width:180px;">
            <img src="~/assets/img/img_173.png"
                 style="top:0;position: absolute;height: 180px;width:180px;">
            <p
              style="position:absolute;top:-10px;left:30px;color: rgb(255, 255, 255);font-family:sans-serif;font-size: 60px;font-weight: 400;line-height: 91px;letter-spacing: 0;">
              农药
            </p>
          </div>
          <div style="bottom:0;position: absolute;height: 180px;width:180px;">
            <img src="~/assets/img/img_174.png"
                 style="bottom:0;position: absolute;height: 180px;width:180px;">
            <p
              style="position:absolute;top:-10px;left:30px;color: rgb(255, 255, 255);font-family:sans-serif;font-size: 60px;font-weight: 400;line-height: 91px;letter-spacing: 0;">
              百货
            </p>
          </div>
        </div>
        <div class="block4"
          style="left:1080px;position: absolute;top:0;height: 400px;width:180px;">
          <div style="top:0;position: absolute;height: 180px;width:180px;">
            <img src="~/assets/img/img_175.png"
                 style="top:0;position: absolute;height: 180px;width:180px;">
            <p
              style="position:absolute;top:-10px;left:30px;color: rgb(255, 255, 255);font-family:sans-serif;font-size: 60px;font-weight: 400;line-height: 91px;letter-spacing: 0;">
              蛋类
            </p>
          </div>
          <div>
            <img src="~/assets/img/img_176.png"
                 style="bottom:0;position: absolute;height: 180px;width:180px;">
            <p
              style="position:absolute;top:200px;left:30px;color: rgb(255, 255, 255);font-family:sans-serif;font-size: 60px;font-weight: 400;line-height: 91px;letter-spacing: 0;">
              禽类
            </p>
          </div>
        </div>
      </div>

    </div>
    <div class="dynamic">
      <div class="tag_dynamic">
        <svg-icon style="font-size: 200px; position: absolute; top: -50px; left: 10px;" icon-class="dynamic"/>
      </div>
      <div class="body"
           style="position: absolute;height: 1580px;width: 1240px;top:100px;left: 40px;">
        <div class="video"
             style="background-color: #F6BE50; position: absolute; top:0px;height: 80px;width: 380px;left: 0px;text-align: center;">
          <svg-icon style="font-size: 80px; position: absolute; top: 0px; left: 10px;" icon-class="video"/>
          <p
            style="position: absolute;left: 150px;top:-25px;font-family: sans-serif;font-size: 40px;vertical-align: center;">
            视 频</p>
        </div>
        <div class="page1"
             style=" position: absolute; top:100px;height: 700px;width: 380px;left: 0px;text-align: center;">
          <div class="button"
               style="position: absolute;z-index: 1">
            <svg-icon style="font-size: 80px; position: absolute; right:-230px;top: 320px;" icon-class="stop"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 20px;" icon-class="hearing1"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 70px;" icon-class="forward2"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 120px;" icon-class="share3"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 170px;" icon-class="heart4"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 220px;" icon-class="commit5"/>
          </div>
          <img src="~/assets/img/img_181.png"
               style="position: absolute; top:0px;height: 700px;width: 380px;left: 0px;">
          <img src="~/assets/img/img_1811.png"
               style="position: absolute; bottom:0px;height: 60px;width: 380px;left: 0px;">

        </div>
        <div class="page2"
             style=" position: absolute; top:0px;height: 700px;width: 380px;left: 430px;text-align: center;">
          <div class="button"
               style="position: absolute;z-index: 1">
            <svg-icon style="font-size: 80px; position: absolute; right:-230px;top: 320px;" icon-class="stop"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 20px;" icon-class="hearing1"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 70px;" icon-class="forward2"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 120px;" icon-class="share3"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 170px;" icon-class="heart4"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 220px;" icon-class="commit5"/>
          </div>

          <img src="~/assets/img/img_182.png"
               style="position: absolute; top:0px;width: 380px;left:0;height: 700px;">
          <img src="~/assets/img/img_1822.png"
               style="position: absolute; bottom:0px;width: 380px;left:0;height: 60px;">
        </div>
        <div class="live"
             style="background-color: #F6BE50; position: absolute; top:0px;height: 80px;width: 380px;right: 0px;text-align: center;">
          <svg-icon style="font-size: 80px; position: absolute; top: 0px; left: 10px;" icon-class="live"/>
          <p
            style="position: absolute;left: 150px;top:-25px;font-family: sans-serif;font-size: 40px;vertical-align: center;">
            直 播</p>
        </div>
        <div class="page3"
             style=" position: absolute; top:100px;height: 700px;width: 380px;right:0;text-align: center;">
          <div class="button"
               style="position: absolute;z-index: 1">
            <svg-icon style="font-size: 80px; position: absolute; right:-230px;top: 320px;" icon-class="stop"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 20px;" icon-class="hearing1"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 70px;" icon-class="forward2"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 120px;" icon-class="share3"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 170px;" icon-class="heart4"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 220px;" icon-class="commit5"/>
          </div>

          <img src="~/assets/img/img_183.png"
               style="position: absolute; top:0px;height: 700px;width: 380px;right:0;">
          <img src="~/assets/img/img_1833.png"
               style="position: absolute; bottom:0px;height:60px;width: 380px;right:0;">
        </div>
        <div class="page4"
             style=" position: absolute; top:840px;height: 700px;width: 380px;left: 0px;text-align: center;">
          <div class="button"
               style="position: absolute;z-index: 1">
            <svg-icon style="font-size: 80px; position: absolute; right:-230px;top: 320px;" icon-class="stop"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 20px;" icon-class="hearing1"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 70px;" icon-class="forward2"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 120px;" icon-class="share3"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 170px;" icon-class="heart4"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 220px;" icon-class="commit5"/>
          </div>

          <img src="~/assets/img/img_184.png"
               style="position: absolute; top:0px;height: 700px;width: 380px;right:0;">
          <img src="~/assets/img/img_1844.png"
               style="position: absolute; bottom:0px;height: 60px;width: 380px;right:0;">
        </div>
        <div class="page5"
             style=" position: absolute; top:740px;height: 700px;width: 380px;left: 430px;text-align: center;">
          <div class="button"
               style="position: absolute;z-index: 1">
            <svg-icon style="font-size: 80px; position: absolute; right:-230px;top: 320px;" icon-class="stop"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 20px;" icon-class="hearing1"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 70px;" icon-class="forward2"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 120px;" icon-class="share3"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 170px;" icon-class="heart4"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 220px;" icon-class="commit5"/>
          </div>
          <img src="~/assets/img/img_185.png"
               style="position: absolute; top:0px;height: 700px;width: 380px;right:0;">
          <img src="~/assets/img/img_1855.png"
               style="position: absolute; bottom:0px;height: 60px;width: 380px;right:0;">
        </div>
        <div class="page6"
             style=" position: absolute; top:840px;height: 700px;width: 380px;right:0;text-align: center;">
          <div class="button"
               style="position: absolute;z-index: 1">
            <svg-icon style="font-size: 80px; position: absolute; right:-230px;top: 320px;" icon-class="stop"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 20px;" icon-class="hearing1"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 70px;" icon-class="forward2"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 120px;" icon-class="share3"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 170px;" icon-class="heart4"/>
            <svg-icon style="font-size: 40px; position: absolute; right:-380px;top: 220px;" icon-class="commit5"/>
          </div>
          <img src="~/assets/img/img_186.png"
               style="position: absolute; top:0px;height: 700px;width: 380px;right:0;">
          <img src="~/assets/img/img_1866.png"
               style="position: absolute; bottom:0px;height: 60px;width: 380px;right:0;">
        </div>
        <div class="查看更多"
             style="background-color: #F6BE50; position: absolute; top:1460px;height: 80px;width: 380px;left: 430px;text-align: center;">
          <p
            style="position: absolute;top:-25px;left: 110px;font-family: sans-serif;font-size: 40px;">
            查看更多</p>
        </div>

      </div>
    </div>
    <div class="orders">
      <div class="tag_order">
        <svg-icon style="font-size: 200px; position: absolute; top: -50px; left: 10px;" icon-class="order"/>
      </div>
      <div class="body"
           style="position: absolute;height: 360px;width: 1240px;top:100px;left: 40px;">
        <div class="block1"
             style="position: absolute;height: 360px;width: 410px;top:0px;left: 0px;">
          <div class="circle"
               style="background: rgba(24, 77, 71, 0.64);position: absolute;border-radius: 130px; height: 260px;width: 260px;left: 75px;top: 20px">
            <svg-icon style="font-size: 180px; position: absolute; top: 40px; left: 40px;" icon-class="manage"/>
          </div>
          <p
            style="position: absolute;bottom: -40px;left:70px;width:260px;height:40px;color: rgb(24, 77, 71);text-align: center; font-family: HappyZcool-2016,sans-serif;font-size: 52px;font-weight: 400;line-height: 59px;letter-spacing: 0px;">
            订单管理
          </p>
        </div>
        <div class="block2"
             style="position: absolute;height: 360px;width: 420px;top:0px;left: 410px;">
          <div class="circle"
               style="background: rgb(246, 190, 80);position: absolute;border-radius: 130px; height: 260px;width: 260px;left: 75px;top: 20px">
            <svg-icon style="font-size: 180px; position: absolute; top: 40px; left: 40px;" icon-class="sell"/>
          </div>
          <p
            style="position: absolute;bottom: -40px;left:70px;width:260px;height:40px;color: rgb(24, 77, 71);text-align: center; font-family: HappyZcool-2016,sans-serif;font-size: 52px;font-weight: 400;line-height: 59px;letter-spacing: 0px;">
            促销管理
          </p>
        </div>
        <div class="block3"
             style="position: absolute;height: 360px;width: 410px;top:0px;right: 0px;">
          <div class="circle"
               style="background: rgb(147, 188, 224);position: absolute;border-radius: 130px; height: 260px;width: 260px;left: 75px;top: 20px">
            <svg-icon style="font-size: 180px; position: absolute; top: 40px; left: 40px;" icon-class="date"/>
          </div>
          <p
            style="position: absolute;bottom: -40px;left:70px;width:260px;height:40px;color: rgb(24, 77, 71);text-align: center; font-family: HappyZcool-2016,sans-serif;font-size: 52px;font-weight: 400;line-height: 59px;letter-spacing: 0px;">
            保质期管理
          </p>
        </div>
      </div>

    </div>
    <div class="income">
      <div class="tag_income">
        <svg-icon style="font-size: 200px; position: absolute; top: -50px; left: 10px;" icon-class="income"/>
      </div>
      <div class="body"
           style="position: absolute;height: 360px;width: 1240px;top:100px;left: 40px;">
        <div class="block1"
             style="position: absolute;height: 360px;width: 310px;top:0px;left: 0px;">
          <div class="square"
               style="background: rgba(246, 190, 80, 0.53);border-radius: 10px;position: absolute;height: 260px;width: 260px;top:0px;left: 0px;">
            <svg-icon style="font-size: 230px; position: absolute; top: 16px; left: 16px;" icon-class="incomeinfo"/>
          </div>
          <div style="top: 300px;background: rgba(246, 190, 80, 0.14);color: rgb(24, 77, 71);border-radius: 9px;height: 60px;width: 260px;position: absolute;text-align: center; font-family: HappyZcool-2016,sans-serif;font-size: 52px;font-weight: 400;line-height: 59px;letter-spacing: 0px;">
            基本情况
          </div>
        </div>
        <div class="block2"
             style="position: absolute;height: 360px;width: 310px;top:0px;left: 310px;">
          <div class="square"
               style="background: rgb(251, 157, 193);border-radius: 10px;position: absolute;height: 260px;width: 260px;top:0px;left: 20px;">
            <svg-icon style="font-size: 230px; position: absolute; top: 16px; left: 16px;" icon-class="product"/>
          </div>
          <div style="top: 300px;background: rgba(246, 190, 80, 0.14);color: rgb(24, 77, 71);left: 20px;border-radius: 9px;height: 60px;width: 260px;position: absolute;text-align: center; font-family: HappyZcool-2016,sans-serif;font-size: 52px;font-weight: 400;line-height: 59px;letter-spacing: 0px;">
            产业结构
          </div>
        </div>
        <div class="block3"
             style="position: absolute;height: 360px;width: 310px;top:0px;left: 620px;">
          <div class="square"
               style="background: rgb(147, 214, 251);border-radius: 10px;position: absolute;height: 260px;width: 260px;top:0px;left: 30px;">
            <svg-icon style="font-size: 230px; position: absolute; top: 16px; left: 16px;" icon-class="dateanalysis"/>
          </div>
          <div style="top: 300px;background: rgba(246, 190, 80, 0.14);color: rgb(24, 77, 71);border-radius: 9px;left: 30px;height: 60px;width: 260px;position: absolute;text-align: center; font-family: HappyZcool-2016,sans-serif;font-size: 52px;font-weight: 400;line-height: 59px;letter-spacing: 0px;">
            季节性分析
          </div>
        </div>
        <div class="block4"
             style="position: absolute;height: 360px;width: 310px;top:0px;right: 0px;">
          <div class="square"
               style="background: rgba(216, 74, 29, 0.73);border-radius: 10px;position: absolute;height: 260px;width: 260px;top:0px;right: 0px;">
            <svg-icon style="font-size: 230px; position: absolute; top: 16px; left: 16px;" icon-class="area"/>
          </div>
          <div style="top: 300px;background: rgba(246, 190, 80, 0.14);color: rgb(24, 77, 71);right:0;border-radius: 9px;height: 60px;width: 260px;position: absolute;text-align: center; font-family: HappyZcool-2016,sans-serif;font-size: 52px;font-weight: 400;line-height: 59px;letter-spacing: 0px;">
            区域情况
          </div>
        </div>
      </div>
    </div>

  </div>
  </main>
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
.main{
  position: relative;
  width: 100%;
  height: 5000px;
  overflow: hidden;
}
/*css 代码*/
/* 矩形 8 */
.supply { /* 矩形 8 */
  position: absolute;
  align-content: center;
  width: 90%;
  height: 700px;
  top: 200px;
  left: 100px;
  background: rgba(215, 245, 109, 0.1);
}

.dynamic { /* 我的动态 */
  position: absolute;
  width: 90%;
  height: 2400px;
  top: 950px;
  left: 100px;
  background: rgba(255, 100, 100, 0.1);
}

.orders {
  /* 订单管理 */
  position: absolute;
  width: 90%;
  height: 700px;
  top: 3500px;
  left: 100px;
  background: rgba(255, 200, 109, 0.1);
}

.income {
  /* 收入分析 */
  position: absolute;
  width: 90%;
  height: 650px;
  top: 4200px;
  left: 100px;
  background: rgba(100, 245, 200, 0.1);
}
</style>
