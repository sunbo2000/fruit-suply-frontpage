<template>
  <div class="page">
    <div class="container">
      <!--      分界线 模块1-->
      <div class="headerItem0">
        <!--        标题-->

        <p class="actionBg">
          基地信息</p>

        <p class="floorBg">
          基地是开展某种活动的基础性地点，犹如某种活动的家园
        </p>
        <!--        内容-->
        <div class="group">
          <!--          模块1.2.1-->
          <div class="viewItem0">

            <div class="item">
              <p class="border"></p>
            </div>
            <p class="logo">
              果园面积
            </p>

            <p class="bg">
              Orchard Area
            </p>
          </div>
          <!--          模块1.2.2-->
          <div class="viewItem1">

            <div class="product">
              <p class="border"></p>
            </div>

            <p class="logo1">
              果园环境
            </p>

            <p class="bg1">
              Orchard Environment
            </p>
          </div>
          <!--          模块1.2.3-->
          <div class="viewItem2">
            <!--            <img-->
            <!--              class="item1"-->
            <!--              src="~assets/trace/img_8.png"-->
            <!--            />-->
            <div class="item1">
              <p class="border"></p>
            </div>

            <p class="logo2">
              果园数量
            </p>

            <p class="bg2">
              Number of Orchard
            </p>
          </div>
        </div>

        <p class="longBg">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore.
          Nulla pellentesque mi non laoreet eleifend. Integer porttitor mollisar lorem, at molestie arcu pulvinar ut.
          Proin ac fermentum est.
        </p>
      </div>
      <!--      分界线 模块2-->
      <div class="headerItem1">

        <p class="buttonBg">
          农事管理
        </p>

        <p class="bar">
          基地是开展某种活动的基础性地点，犹如某种活动的家园
        </p>
        <!--        模块2.2-->
        <div class="grid">
          <!--          模块2.2.1-->
          <div class="colItem0">


            <div class="itemLong">
              <div class="circle1">
                <!--              插入图片-->

              </div>
              <div class="square">
                播种
              </div>
            </div>

            <p class="actionBg1">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore.
            </p>
          </div>
          <!--        模块2.2.2-->
          <div class="colItem1">

            <div class="itemLong">
              <div class="circle1">
                <!--              插入图片-->

              </div>
              <div class="square">
                土壤
              </div>
            </div>
            <div class="buttonBg1">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore.
            </div>
          </div>
          <!--          模块2.2.3-->
          <div class="colItem2">
            <div class="itemLong">
              <div class="circle1">
                <!--              插入图片-->

              </div>
              <div class="square">
                施肥
              </div>
            </div>

            <div class="actionBg2">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore.
            </div>
          </div>

        </div>
      </div>

      <!--      分界线 模块3-->
      <div class="main">
        <!--        3.1   -->
        <div class="group1">

          <p class="buttonBg4">
            出入库记录
          </p>

          <p class="atmosphere">
            基地是开展某种活动的基础性地点，犹如某种活动的家园
          </p>
        </div>

        <!--        3.2.1-->
        <div class="groupItem0">
          <div class="backgroundWrapperItem0">
            <div class="largeIcon">
              时间
            </div>
            <div class="buttonBg2">
              Nulla pellentesque mi non laoreet eleifend. Integer porttitor mollisar lorem, at molestie arcu pulvinar
              ut.
            </div>
            <div class="entryPic">
              <!--图片-->
            </div>
            <div class="background2">

            </div>

          </div>
          <div class="backgroundWrapperItem1">
            <div class="largeIcon">
              数量
            </div>
            <div class="buttonBg2">
              Nulla pellentesque mi non laoreet eleifend. Integer porttitor mollisar lorem, at molestie arcu pulvinar
              ut.
            </div>
            <div class="entryPic">
              <!--图片-->
            </div>
            <div class="background2">

            </div>
          </div>
        </div>

        <!--        模块3.2.2-->
        <div class="groupItem1">
          <div class="backgroundWrapperItem01">

            <div class="largeIcon">
              品种
            </div>
            <div class="buttonBg2">
              Nulla pellentesque mi non laoreet eleifend. Integer porttitor mollisar lorem, at molestie arcu pulvinar
              ut.
            </div>
            <div class="entryPic">
              <!--图片-->
            </div>
            <div class="background2">

            </div>
          </div>
          <div class="backgroundWrapperItem11">

            <div class="largeIcon">
              重量
            </div>
            <div class="buttonBg2">
              Nulla pellentesque mi non laoreet eleifend. Integer porttitor mollisar lorem, at molestie arcu pulvinar
              ut.
            </div>
            <div class="entryPic">
              <!--图片-->
            </div>
            <div class="background2">

            </div>
          </div>
        </div>

      </div>
    </div>
  </div>

</template>
export default {
components: {

},
data() {
return {
constants: {}
}
},
methods: {

},

}


<script>
export default {
  name: "index.vue"
}
</script>

<style scoped>
.page {
  width: 1980px;
  height: 3050px;
}

.page .container {
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}

.page .headerItem0 {
  background-size: contain;
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: column;
  background-color: #efefef;
  width: 1980px;
  height: 1050px;
  overflow: hidden;
}

.page .actionBg {
  position: relative;
  margin-top: 107px;
  width: 258px;
  height: 68px;
  /*background-color: red;*/
  text-align: center;
  color: #046d32;
  font-size: 52px;
  /*line-height: 1em;*/
  font-weight: 700;
  /*letter-spacing: 0.04em;*/
  text-transform: capitalize;
}

.page .floorBg {
  position: relative;
  margin-top: -10px;
  padding-top: 10px;
  text-align: center;
  letter-spacing: 8px;
  width: 1007px;
  height: 45px;
  color: #696969;
  font-size: 25px;
  font-weight: 700;
  /*background-color: aliceblue;*/
}

.page .group {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  margin-top: 21px;
}

.page .viewItem0 {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: row;
  justify-content: center;
}

.page .item {
  position: relative;
  width: 493px;
  height: 492px;
  /*background-color: #777777;*/
}

.page .border {
  position: absolute;
  top: 60px;
  left: 19px;
  height: 296px;
  width: 455px;
  background-color: rgba(10,255,20,0.3);
  border-radius: 10px;
}

.page .logo {
  position: absolute;
  font-size: 25px;
  font-weight: 600;
  color: #404248;
  bottom: 40px;
  left: 19px;
  width: 124px;
  height: 30px;
  /*background-color: aliceblue;*/

}

.page .bg {
  position: absolute;
  width: 300px;
  bottom: 15px;
  left: 19px;
  height: 30px;
  font-size: 20px;
  font-weight: 600;
  color: #696969;
  letter-spacing: 4px;
  /*background-color: aliceblue;*/

}


.page .viewItem1 {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: row;
  justify-content: center;
}

.page .product {
  position: relative;
  width: 493px;
  height: 492px;
  /*background-color: #777777;*/

}

.page .logo1 {
  position: absolute;
  font-size: 25px;
  font-weight: 600;
  color: #404248;
  bottom: 40px;
  left: 19px;
  width: 124px;
  height: 30px;
  /*background-color: aliceblue;*/

}

.page .bg1 {
  position: absolute;
  width: 300px;
  bottom: 15px;
  left: 19px;
  height: 30px;
  font-size: 20px;
  font-weight: 600;
  color: #696969;
  letter-spacing: 4px;
  /*background-color: aliceblue;*/
}

.page .viewItem2 {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: row;
  justify-content: center;
}

.page .item1 {
  position: relative;
  width: 493px;
  height: 492px;
  /*background-color: #777777;*/

}

.page .logo2 {
  position: absolute;
  font-size: 25px;
  font-weight: 600;
  color: #404248;
  bottom: 40px;
  left: 19px;
  width: 124px;
  height: 30px;
  /*background-color: aliceblue;*/

}

.page .bg2 {
  position: absolute;
  bottom: 15px;
  width: 300px;
  left: 19px;
  height: 30px;
  font-size: 20px;
  font-weight: 600;
  color: #696969;
  letter-spacing: 4px;
  /*background-color: aliceblue;*/
}

.page .longBg {
  position: relative;
  margin-top: 44px;
  width: 1471px;
  height: 80px;
  font-size: 20px;
  font-weight: 400;
  text-align: center;
  /*background-color: aliceblue;*/
  line-height: 35px;
  color: #777777;
}

.page .headerItem1 {
  background-size: contain;
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: column;
  /*background-color: #ffffff;*/
  width: 1980px;
  height: 900px;
}

.page .buttonBg {

  position: relative;
  margin-top: 107px;
  width: 258px;
  height: 68px;
  /*background-color: aliceblue;*/
  text-align: center;
  color: #046d32;
  font-size: 52px;
  /*line-height: 1em;*/
  font-weight: 700;
  /*letter-spacing: 0.04em;*/
  text-transform: capitalize;
}

.page .bar {
  position: relative;
  margin-top: -10px;
  padding-top: 10px;
  text-align: center;
  letter-spacing: 8px;
  width: 1007px;
  height: 45px;
  color: #696969;
  font-size: 25px;
  font-weight: 700;
  /*background-color: aliceblue;*/
}

.page .grid {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  margin-top: 29px;
}

.page .colItem0 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: column;
  /*border-width: 1px;*/
  /*border-style: solid;*/
  width: 492px;
  height: 497px;
}


.page .itemLong {
  position: relative;
  margin-top: 69px;
  width: 188px;
  height: 242px;
}

.page .circle1 {
  position: absolute;
  width: 140px;
  height: 140px;
  border-radius: 94px;
  top: 0;
  left: 24px;
  border: 1px dashed #046d32;
  background-color: rgba(10,255,20,0.3);

}

.page .square {
  position: absolute;
  width: 140px;
  height: 45px;
  bottom: 10px;
  left: 24px;
  font-size: 30px;
  font-weight: 600;
  color: #212121;
  text-align: center;
}

.page .actionBg1 {
  position: relative;
  margin-top: 36px;
  width: 468px;
  height: 114px;
  /*background-color: rgba(0, 255, 20, 0.4);*/
  font-size: 20px;
  letter-spacing: 2px;
  text-align: center;
  line-height: 35px;
  font-weight: 400;
  color: #777777;
}

.page .colItem1 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: column;
  /*border-width: 1px;*/
  /*border-style: solid;*/
  /*border-color: rgba(0, 0, 0, 1);*/
  width: 492px;
  height: 497px;
}


.page .buttonBg1 {
  position: relative;
  margin-top: 36px;
  width: 468px;
  height: 114px;
  /*background-color: rgba(0, 255, 20, 0.4);*/
  font-size: 20px;
  letter-spacing: 2px;
  text-align: center;
  line-height: 35px;
  font-weight: 400;
  color: #777777;
}

.page .colItem2 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: column;
  /*border-width: 1px;*/
  /*border-style: solid;*/
  /*border-color: rgba(0, 0, 0, 1);*/
  width: 492px;
  height: 497px;
}

.page .actionBg2 {
  position: relative;
  margin-top: 36px;
  width: 468px;
  height: 114px;
  /*background-color: rgba(0, 255, 20, 0.4);*/
  font-size: 20px;
  letter-spacing: 2px;
  text-align: center;
  line-height: 35px;
  font-weight: 400;
  color: #777777;
}

.page .main {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: row;
  justify-content: center;
  width: 1980px;
}

.page .groupItem0 {
  display: flex;
  position: absolute;
  top: 630px;
  left: 252px;
  align-items: center;
  flex-direction: row;
  width: 1476px;
  height: 294px;
}

.page .backgroundWrapperItem0 {
  display: flex;
  position: absolute;
  top: 0px;
  left: 0px;
  align-items: center;
  flex-direction: row;
  width: 738px;
  height: 294px;
}

.page .largeIcon {
  position: absolute;
  top: 51px;
  left: 327px;
  width: 69px;
  height: 47px;
  position: absolute;
  font-size: 25px;
  font-weight: 600;
  color: #404248;
  bottom: 40px;
  /*left: 19px;*/
  /*width: 124px;*/
  /*height: 30px;*/
  /*background-color: aliceblue;*/
}

.page .buttonBg2 {
  position: absolute;
  top: 114px;
  right: 50px;
  width: 361px;
  height: 108px;
  color: #777777;
  font-size: 20px;
  font-weight: 400;
  /*background-color: aliceblue;*/
  line-height: 35px;
}

.page .entryPic {
  position: absolute;
  top: 51px;
  left: 18px;
  width: 278px;
  height: 185px;
  background-color: rgba(10,255,20,0.3);
  border-radius: 10px;
}

.page .background2 {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 738px;
  height: 294px;
  /*background-color: rgba(10, 255, 0, 0.2);*/
}

.page .backgroundWrapperItem1 {
  display: flex;
  position: absolute;
  top: 0px;
  right: 0px;
  align-items: center;
  flex-direction: row;
  width: 738px;
  height: 294px;
}



.page .groupItem1 {
  display: flex;
  position: absolute;
  top: 336px;
  left: 252px;
  align-items: center;
  flex-direction: row;
  width: 1476px;
  height: 294px;
}

.page .backgroundWrapperItem01 {
  display: flex;
  position: absolute;
  top: 0px;
  left: 0px;
  align-items: center;
  flex-direction: row;
  width: 738px;
  height: 294px;
}


.page .backgroundWrapperItem11 {
  display: flex;
  position: absolute;
  top: 0px;
  right: 0px;
  align-items: center;
  flex-direction: row;
  width: 738px;
  height: 294px;
}


.page .group1 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: column;
  background-size: contain;
  background-color: #efefef;
  width: 1977px;
  height: 1100px;
}

.page .buttonBg4 {
  position: relative;
  margin-top: 107px;
  width: 308px;
  height: 68px;
  /*background-color: aliceblue;*/
  text-align: center;
  color: #046d32;
  font-size: 52px;
  /*line-height: 1em;*/
  font-weight: 700;
  /*letter-spacing: 0.04em;*/
  text-transform: capitalize;

}

.page .atmosphere {
  position: relative;
  margin-top: -10px;
  padding-top: 10px;
  text-align: center;
  letter-spacing: 8px;
  width: 1007px;
  height: 45px;
  color: #696969;
  font-size: 25px;
  font-weight: 700;
  /*background-color: aliceblue;*/
}


</style>
