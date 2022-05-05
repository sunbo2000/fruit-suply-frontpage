<template>
  <el-main class="pbmMain">
    <div class="mod">
      <div class="group">

        <div class="actionBgWrapper">
          <img class="actionBg" src="~/assets/img1/img_0.png" alt=""/>
          <span class="title">智能灌溉系统</span>
        </div>

        <div class="actionBgWrapperItem01">
          <img class="actionBg1" src="~/assets/img1/img_6.png"
          />
          <span class="title2">智能大棚系统</span>
        </div>

        <div class="textBackgroundWrapper">
          <img
            class="textBackground"
            src="~/assets/img1/img_1.png"
          />
          <span class="caption">气象站数据集中采集系统</span>
        </div>

        <img class="buttonBg" src="~/assets/img1/img_4.png"/>
        <span class="title1">农业大数据分析系统</span>
        <img class="textBackground1" src="~/assets/img1/img_2.png"/>
        <img
          class="iconDown"
          src="~/assets/img1/img_3.png"
        />

        <div class="main">

          <div class="floorBgWrapper">
            <img class="floorBg" src="~/assets/img1/img_5.png"/>

          </div>
          <div class="longBgWrapper">
            <img class="longBg" src="~/assets/img1/img_7.png"/>
            <div class="container">
              <img class="horizontalLine" src="~/assets/img1/img_8.png"/>
              <div class="wrapper">
                <img class="badge" src="~/assets/img1/img_9.png"/>
                <img class="figure" src="~/assets/img1/img_10.png"/>
              </div>
            </div>
            <span class="caption2">系统分析</span>
          </div>
          <div class="block1">


            <div class="container2">

              <div class="wrapperItem0">

                <div class="bottom222">

                <span class="caption13">
                  <img class="ha" src="~/assets/img1/img_30.png" alt="温度"/>
                  <font class="font111">温度</font>
                </span>
                </div>

                <div class="bottom333">

                <span class="caption13">
                  <img class="ha" src="~/assets/img1/img_20.png" alt="UV"/>
                  <font class="font111">UV</font>
                </span>
                </div>
                <div class="bottom222">

                <span class="caption13">
                  <img class="ha" src="~/assets/img1/img_31.png" alt="虫害"/>
                  <font class="font111">虫害</font>
                </span>
                </div>
                <div class="bottom333">

                 <span class="caption13">
                  <img class="ha" src="~/assets/img1/img_37.png" alt="风速"/>
                  <font class="font111">风速</font>
                </span>
                </div>
                <div class="bottom222">

                <span class="caption13">
                  <img class="ha" src="~/assets/img1/img_21.png" alt="湿度"/>
                  <font class="font111">湿度</font>
                </span>
                </div>
                <div class="bottom333">

                 <span class="caption13">
                  <img class="ha" src="~/assets/img1/img_22.png" alt="气压"/>
                  <font class="font111">气压</font>
                </span>
                </div>
              </div>

            </div>


            <img
              class="banner"
              src="~/assets/img1/img_23.png"
            />
            <div class="container3">
              <img
                class="background"
                src="~/assets/img1/img_24.png"
              />
              <img
                class="cover"
                src="~/assets/img1/img_25.png"
              />
              <img
                class="banner1"
                src="~/assets/img1/img_26.png"
              />
            </div>
            <div class="container4">
              <img
                class="layer1"
                src="~/assets/img1/img_27.png"
              />
              <div class="wrapper1">

              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </el-main>
</template>
<script>


export default {
  layout: 'admin',
  components: {},
  data() {
    return {
      constants: {}
    }
  },
  methods: {},

}
</script>
<style scoped>
.pbmMain{
  width: 1460px;
  margin: 0;
  padding: 0;
  border: 0;
}
.mod {
  margin-top: 56px;
  width: 1460px;
  height: 1980px;
}

.mod .group {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  width: 1460px;
  height: 1700px;
  position: relative;
  top: 20px;
  left: -90px;
  background-color: #ffffff;
}

.mod .actionBgWrapper {
  display: flex;
  position: absolute;
  top: 106px;
  left: 750px;
  align-items: center;
  flex-direction: row;
  width: 205px;
  height: 46px;
}

.mod .actionBg {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 205px;
  height: 46px;
}

.mod .title {
  position: absolute;
  bottom: -1px;
  left: 0px;
  line-height: 45px;
  letter-spacing: 2px;
  white-space: nowrap;
  color: #184d47;
  font-size: 30px;
  font-weight: 400;
  z-index: 1;
}

.mod .textBackgroundWrapper {
  display: flex;
  position: absolute;
  top: 103px;
  left: 970px;
  align-items: center;
  flex-direction: row;
  width: 372px;
  height: 50px;
}

.mod .textBackground {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 363px;
  height: 50px;
}

.mod .caption {
  position: absolute;
  bottom: 0px;
  left: 5px;
  line-height: 45px;
  letter-spacing: 2px;
  white-space: nowrap;
  color: #184d47;
  font-size: 30px;
  font-weight: 400;
  z-index: 1;
}

.mod .title1 {
  position: absolute;
  top: 109px;
  left: 200px;
  line-height: 45px;
  letter-spacing: 2px;
  white-space: nowrap;
  color: #a84a07;
  font-size: 30px;
  font-weight: 400;
  z-index: 1;
}

.mod .textBackground1 {
  position: absolute;
  top: 155px;
  left: 195px;
  width: 298px;
  height: 9px;
}

.mod .iconDown {
  position: absolute;
  top: 156px;
  left: 325px;
  width: 20px;
  height: 20px;
}

.mod .main {
  display: flex;
  position: relative;
  align-items: flex-start;
  align-self: center;
  flex-direction: row;
}

.mod .buttonBg {
  position: absolute;
  top: 100px;
  left: 200px;
  width: 300px;
  height: 55px;
}

.mod .floorBgWrapper {
  display: flex;
  position: absolute;
  top: 100px;
  right: 35px;
  align-items: center;
  flex-direction: row;
  width: 1137px;
  height: 55px;
}

.mod .floorBg {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 1137px;
  height: 55px;
}

.mod .actionBg1 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 205px;
  height: 50px;
}

.mod .title2 {
  position: absolute;
  top: 2px;
  line-height: 45px;
  letter-spacing: 2px;
  white-space: nowrap;
  color: #184d47;
  font-size: 30px;
  font-weight: 400;
  z-index: 1;
}

.mod .longBgWrapper {
  display: flex;
  position: absolute;
  top: 0px;
  right: 17px;
  align-items: center;
  flex-direction: row;
  width: 1243px;
  height: 105px;
}

.mod .longBg {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 1243px;
  height: 105px;
}

.mod .container {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
  margin-top: 1px;
  margin-right: 18px;
  margin-left: 17px;
  width: 66px;
  height: 80px;
  overflow: hidden;
}

.mod .horizontalLine {
  position: relative;
  margin-top: 20px;
  margin-left: 6px;
  width: 33px;
  height: 7px;
}

.mod .wrapper {
  display: flex;
  position: relative;
  align-items: flex-start;
  align-self: center;
  flex-direction: row;
  justify-content: center;
  margin-top: 6px;
}

.mod .badge {
  position: relative;
  width: 55px;
  height: 33px;
}

.mod .figure {
  position: absolute;
  top: 14px;
  left: 0px;
  width: 22px;
  height: 7px;
}

.mod .caption2 {
  position: relative;
  line-height: 40px;
  letter-spacing: 2px;
  white-space: nowrap;
  color: #ffffff;
  font-size: 40px;
  font-weight: 400;
}

.mod .block {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
  margin-right: 18px;
}

.mod .container1 {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
  background-size: contain;
  background-image: url("~/assets/img1/img_32.png");
  width: 300px;
  height: 754px;
}

.mod .buttonBgWrapper {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: row;
  justify-content: center;
  width: 300px;
  height: 118px;
}

.mod .buttonBg1 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 105px;
}

.mod .title3 {
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


.mod .actionBgWrapperItem0 {
  display: flex;
  position: relative;
  margin-top: 20px;
  align-items: center;
  flex-direction: row;
  width: 300px;
  height: 71px;
}

.mod .actionBgWrapperItem01 {
  display: flex;
  position: absolute;
  background-color: black;
  top: 106px;
  left: 520px;
}

.mod .actionBg2 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.mod .caption3 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  text-overflow: ellipsis;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
}


.mod .buttonBg2 {
  position: absolute;
  left: 0px;
  width: 300px;
  height: 71px;
}

.mod .caption04 {
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

.mod .actionBg3 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.mod .caption5 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  overflow: hidden;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
}

.mod .buttonBg3 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.mod .caption6 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  overflow: hidden;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
}

.mod .actionBg4 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.mod .caption7 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  overflow: hidden;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
}

.mod .buttonBg4 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.mod .caption8 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  overflow: hidden;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
}

.mod .title9 {
  position: absolute;
  top: 545px;
  left: 48px;
  line-height: 60px;
  letter-spacing: 15px;
  white-space: nowrap;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
}

.mod .actionBgWrapperItem5 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  margin-top: 19px;
  width: 300px;
  height: 71px;
}

.mod .actionBg5 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 71px;
}

.mod .caption9 {
  position: relative;
  margin-top: -2px;
  margin-left: 48px;
  max-width: 204px;
  overflow: hidden;
  line-height: 40px;
  letter-spacing: 15px;
  white-space: nowrap;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
}

.mod .title10 {
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

.mod .caption10 {
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

.mod .layer {
  position: relative;
  margin-top: 40px;
  width: 300px;
  height: 1028px;
}

.mod .block1 {
  display: flex;
  position: relative;
  left: -15px;
  align-items: flex-start;
  flex-direction: column;
  margin-top: 103px;
  background-size: contain;
  background-image: url("~/assets/img1/img_33.png");
  width: 1243px;
  height: 1725px;
}

.mod .container2 {
  /* 矩形 17 */
  position: absolute;
  width: 293px;
  height: 470px;
  top: 1250px;
  left: 950px;

  background-color: rgba(40, 63, 6, 0.35);
}

.mod .wrapperItem0 {

}

.mod .group1 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  margin-top: 1px;
  width: 98px;
  height: 120px;
}

.mod .picture {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 98px;
  height: 120px;
}

.mod .title11 {
  position: relative;
  margin-top: -1px;
  max-width: 86px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 50px;
  white-space: nowrap;
  color: #184d47;
  font-size: 50px;
  font-weight: 400;
}


.mod .colItem1 {
  display: flex;
  align-items: center;
  flex-direction: row;
  margin-top: -1px;
  background-size: contain;
  background-image: url("~/assets/img1/img_39.png");
  width: 135px;
  height: 135px;
}

.mod .view1 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  margin-top: 2px;
  margin-left: 9px;
  width: 116px;
  height: 105px;
}

.mod .figure1 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 116px;
  height: 105px;
}

.mod .caption12 {
  position: relative;
  margin-left: 9px;
  max-width: 102px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 50px;
  white-space: nowrap;
  color: #184d47;
  font-size: 50px;
  font-weight: 400;
}

.mod .banner {
  position: relative;
  align-self: flex-end;
  margin-top: 109px;
  margin-right: 17px;
  width: 1137px;
  height: 429px;
}

.mod .container3 {
  display: flex;
  position: relative;
  align-items: center;
  align-self: flex-end;
  flex-direction: row;
  justify-content: center;
  margin-top: 75px;
  margin-right: 18px;
}

.mod .background {
  position: absolute;
  top: 6px;
  left: 0px;
  width: 586px;
  height: 547px;
}

.mod .cover {
  position: relative;
  margin-right: 12px;
  width: 598px;
  height: 559px;
  opacity: 0.6;
}

.mod .banner1 {
  position: relative;
  width: 526px;
  height: 547px;
}

.mod .container4 {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: row;
  margin-top: 76px;
  margin-left: 89px;
}

.mod .layer1 {
  margin-right: 29px;
  width: 798px;
  height: 470px;
}

.mod .wrapper1 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: column;
  margin-top: 8px;
  width: 168px;
}

.mod .groupItem0 {
  display: flex;
  position: absolute;
  bottom: 21px;
  align-items: center;
  align-self: center;
  flex-direction: row;
  width: 135px;
  height: 135px;
}

.mod .bitmap {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 135px;
  height: 135px;
}

.mod .title13 {
  position: absolute;
  top: 42px;
  left: 17px;
  line-height: 58px;
  white-space: nowrap;
  color: #184d47;
  font-size: 50px;
  font-weight: 400;
  z-index: 1;
}

.mod .groupItem1 {
  display: flex;
  position: absolute;
  top: -330px;
  align-items: center;
  align-self: center;
  flex-direction: row;
  width: 135px;
  height: 135px;

  background-color: #184d47;
}

.mod .picture1 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 135px;
  height: 135px;
}

.mod .caption13 {
}

.bottom222 {
  /* 椭圆 1 */
  display: inline-block;
  position: relative;
  width: 135px;
  height: 135px;
  border-radius: 50%;
  margin-right: 17px;
  margin-top: 15px;
  text-align: center;

  background-color: rgba(239, 244, 136, 0.27);
}

.bottom333 {
  /* 椭圆 1 */
  display: inline-block;
  position: relative;
  width: 135px;
  height: 135px;
  border-radius: 50%;
  text-align: center;

  background-color: rgba(239, 244, 136, 0.27);
}

.ha {
  /* 温度 1 */
  position: absolute;
  top: 10px;
  left: 20px;
  border-radius: 50%;
  width: 100px;
  height: 100px;
}

.font111 {
  /* 温度 */
  position: absolute;
  top: 30px;
  left: 20px;
  width: 100px;
  height: 57px;

  color: rgb(24, 77, 71);
  font-family: 楷体, serif;
  font-size: 50px;
  font-weight: 1000;
  line-height: 57px;
  letter-spacing: 0px;
  z-index: 1;
}
</style>
