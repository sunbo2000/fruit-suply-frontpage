<template>
  <div class="mod">
    <div class="container">
      <div class="main">
        <p class="floorBg"></p>

        <div class="actionBgWrapperItem0">
          <p class="actionBg"></p>
          <span class="title">相关政策</span>
        </div>
        <div class="actionBgWrapperItem1">
          <p class="buttonBg"></p>

          <span class="caption">土壤数据</span>
        </div>
        <div class="actionBgWrapperItem2">
          <p class="actionBg1"></p>
          <span class="title1">地理位置</span>
        </div>
        <div class="actionBgWrapperItem3">
          <p class="buttonBg1"></p>
          <span class="caption1">种植作物</span>
        </div>
        <div class="actionBgWrapperItem4">
          <p class="actionBg2"></p>
          <span class="title2">环境数据</span>
        </div>
      </div>
      <img
        class="buttonBg2"
        src="~/assets/government/img_6.png"
      />
      <div class="wrapper">
        <img
          class="iconPlay"
          src="~/assets/government/img_7.png"
        />
      </div>
      <div class="captionWrapperItem0">
        <span class="caption2">相关政策</span>
      </div>
      <div class="wrapper1">
        <div class="group">
          <div class="longBgWrapperItem0">
            <p class="longBg"></p>
            <span class="title3">— 政策文件库 —</span>
          </div>
          <div class="longBgWrapperItem1">
            <p class="bar"></p>

            <span class="caption3">— 政策问答平台 —</span>
          </div>
        </div>
        <div class="slider">
          <el-carousel indicator-position="outside" class="pointer">
            <el-carousel-item v-for="(items,index) in commentList" :key="index">
              <h3 class="medium">
                <div style="line-height: 28px">
                  <p class="summary">&nbsp;{{ items.summary1 }}</p>
                  <p class="summary">&nbsp;{{ items.summary2 }}</p>
                  <p class="summary">&nbsp;{{ items.summary3 }}</p>
                  <p class="summary">&nbsp;{{ items.summary4 }}</p>
                </div>
              </h3>
            </el-carousel-item>
          </el-carousel>
        </div>
      </div>
      <img
        class="iconPlay2"
        src="~/assets/government/img_14.png"
      />
      <div class="captionWrapperItem1">
        <span class="caption7">种植作物</span>
      </div>
      <div class="wrapper2">
        <p class="layer"></p>
        <!--
                <span class="title8">葡萄</span>
                <span class="caption8">柠檬</span>
                <span class="title9">苹果</span>
                <span class="caption9">萝卜</span>-->
        <!--        <span class="title10">种类分析</span>
                <span class="caption10">产量分析</span>
                <span class="title11">销售量</span>
                <span class="caption11">好评率</span>-->
        <el-carousel arrow="never" :interval="4000" class="choose1">
          <el-carousel-item v-for="(items,index) in commentList1" :key="index">
            <h3 class="medium">

              <div class="outer1">
                <img :src="require('~/assets/government/'+items[0].avatar)" class="photo1"/>
                <p class="text1">{{ items[0].content }}</p>
              </div>

              <div class=" outer2">
                <img :src="require('~/assets/government/'+items[1].avatar)" class="photo1"/>
                <p class="text1">{{ items[1].content }}</p>
              </div>

              <div class="outer3">
                <img :src="require('~/assets/government/'+items[2].avatar)" class="photo1"/>
                <p class="text1">{{ items[2].content }}</p>
              </div>

              <div class="outer4">
                <img :src="require('~/assets/government/'+items[3].avatar)" class="photo1"/>
                <p class="text1">{{ items[3].content }}</p>
              </div>

            </h3>
          </el-carousel-item>
        </el-carousel>
        <el-carousel arrow="never" :interval="4000" class="choose2">
          <el-carousel-item v-for="(items,index) in commentList2" :key="index">
            <h3 class="medium">

              <div class="out1">
                <img :src="require('~/assets/government/'+items[0].avatar)" class="photo2"/>
                <p class="text2">{{ items[0].content }}</p>
              </div>

              <div class="out2">
                <img :src="require('~/assets/government/'+items[1].avatar)" class="photo2"/>
                <p class="text2">{{ items[1].content }}</p>
              </div>

              <div class="out3">
                <img :src="require('~/assets/government/'+items[2].avatar)" class="photo2"/>
                <p class="text2">{{ items[2].content }}</p>
              </div>

              <div class="out4">
                <img :src="require('~/assets/government/'+items[3].avatar)" class="photo2"/>
                <p class="text2">{{ items[3].content }}</p>
              </div>

            </h3>
          </el-carousel-item>
        </el-carousel>
      </div>
    </div>
  </div>
</template>
<script>


export default {
  components: {},
  data() {
    return {
      commentList2: [
        [{
          avatar: "img_30.png",
          content: '种植分析',
        },
          {
            avatar: 'img_31.png',
            content: '产量分析',
          },
          {
            avatar: 'img_32.png',
            content: '销售量',
          },
          {
            avatar: 'img_33.png',
            content: '好评率',
          },
        ],
        [{
          avatar: "img_30.png",
          content: '种植分析',
        },
          {
            avatar: 'img_31.png',
            content: '产量分析',
          },
          {
            avatar: 'img_32.png',
            content: '销售量',
          },
          {
            avatar: 'img_33.png',
            content: '好评率',
          },
        ],
        [{
          avatar: "img_30.png",
          content: '种植分析',
        },
          {
            avatar: 'img_31.png',
            content: '产量分析',
          },
          {
            avatar: 'img_32.png',
            content: '销售量',
          },
          {
            avatar: 'img_33.png',
            content: '好评率',
          },
        ],
      ],
      commentList1: [
        [{
          avatar: "img_26.png",
          content: '葡萄',
        },
          {
            avatar: 'img_27.png',
            content: '柠檬',
          },
          {
            avatar: 'img_28.png',
            content: '苹果',
          },
          {
            avatar: 'img_29.png',
            content: '萝卜',
          },
        ],
        [{
          avatar: "img_26.png",
          content: '葡萄',
        },
          {
            avatar: 'img_27.png',
            content: '柠檬',
          },
          {
            avatar: 'img_28.png',
            content: '苹果',
          },
          {
            avatar: 'img_29.png',
            content: '萝卜',
          },
        ],
        [{
          avatar: "img_26.png",
          content: '葡萄',
        },
          {
            avatar: 'img_27.png',
            content: '柠檬',
          },
          {
            avatar: 'img_28.png',
            content: '苹果',
          },
          {
            avatar: 'img_29.png',
            content: '萝卜',
          },
        ],
      ],
      commentList: [
        {
          summary1: ' •《关于全面推进乡村振兴加快农业农村现代化的意见》',
          summary2: ' •《国务院关于加快推进农业机械化和农机装备产业转型升级的指导意见》',
          summary3: ' •《中央财政农业保险保险费补贴管理办法》',
          summary4: ' •《关于促进小农户和现代农业发展有机衔接的意见》',
        },
        {
          summary1: ' •《关于全面推进乡村振兴加快农业农村现代化的意见》',
          summary2: ' •《国务院关于加快推进农业机械化和农机装备产业转型升级的指导意见》',
          summary3: ' •《中央财政农业保险保险费补贴管理办法》',
          summary4: ' •《关于促进小农户和现代农业发展有机衔接的意见》',
        },
        {
          summary1: ' •《关于全面推进乡村振兴加快农业农村现代化的意见》',
          summary2: ' •《国务院关于加快推进农业机械化和农机装备产业转型升级的指导意见》',
          summary3: ' •《中央财政农业保险保险费补贴管理办法》',
          summary4: ' •《关于促进小农户和现代农业发展有机衔接的意见》',
        },
        {
          summary1: ' •《关于全面推进乡村振兴加快农业农村现代化的意见》',
          summary2: ' •《国务院关于加快推进农业机械化和农机装备产业转型升级的指导意见》',
          summary3: ' •《中央财政农业保险保险费补贴管理办法》',
          summary4: ' •《关于促进小农户和现代农业发展有机衔接的意见》',
        },

      ]
    }
  },
  methods: {},

}
</script>

<style scoped>
.mod {
  top: -16px;
  position: relative;
  width: 1920px;
  height: 2200px;
}

.mod .container {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
  background-color: #ffffff;
  height: 3964px;
}

.mod .main {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  width: 1920px;
}

.mod .floorBg {
  position: absolute;
  top: -18px;
  left: 0px;
  width: 1920px;
  height: 73px;
  background: rgb(215, 245, 109);
}

.mod .actionBgWrapperItem0 {
  display: flex;
  position: absolute;
  top: 0px;
  left: 373px;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  width: 239px;
  height: 73px;
}

.mod .actionBg {
  position: absolute;
  top: -18px;
  left: 0px;
  width: 239px;
  height: 73px;
  background: rgba(238, 187, 77, 0.25);
}

.mod .title {
  position: relative;
  max-width: 227px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 36px;
  white-space: nowrap;
  color: #184d47;
  font-size: 36px;
  font-weight: 400;
}

.mod .actionBgWrapperItem1 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  margin-right: 233px;
  margin-left: 845px;
  width: 239px;
  height: 73px;
}

.mod .buttonBg {
  position: absolute;
  top: -18px;
  left: 0px;
  width: 239px;
  height: 73px;
  background: rgba(238, 187, 77, 0.25);
}

.mod .caption {
  position: relative;
  max-width: 227px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 36px;
  white-space: nowrap;
  color: #184d47;
  font-size: 36px;
  font-weight: 400;
}

.mod .actionBgWrapperItem2 {
  display: flex;
  position: absolute;
  top: 0px;
  left: 609px;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  width: 239px;
  height: 73px;
}

.mod .actionBg1 {
  position: absolute;
  top: -18px;
  left: 0px;
  width: 239px;
  height: 73px;
  background: rgba(238, 187, 77, 0.25);
}

.mod .title1 {
  position: relative;
  max-width: 227px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 36px;
  white-space: nowrap;
  color: #184d47;
  font-size: 36px;
  font-weight: 400;
}

.mod .actionBgWrapperItem3 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  width: 239px;
  height: 73px;
}

.mod .buttonBg1 {
  position: absolute;
  top: -18px;
  left: 0px;
  width: 239px;
  height: 73px;
  background: rgba(238, 187, 77, 0.25);
}

.mod .caption1 {
  position: relative;
  max-width: 227px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 36px;
  white-space: nowrap;
  color: #184d47;
  font-size: 36px;
  font-weight: 400;
}

.mod .actionBgWrapperItem4 {
  display: flex;
  position: absolute;
  top: 0px;
  right: 600px;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  width: 239px;
  height: 73px;
}

.mod .actionBg2 {
  position: absolute;
  top: -18px;
  left: 0px;
  width: 239px;
  height: 73px;
  background: rgba(238, 187, 77, 0.25);
}

.mod .title2 {
  position: relative;
  max-width: 227px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 36px;
  white-space: nowrap;
  color: #184d47;
  font-size: 36px;
  font-weight: 400;
}

.mod .buttonBg2 {
  position: relative;
  margin-top: 71px;
  margin-left: 293px;
  width: 161px;
  height: 44px;
}

.mod .wrapper {
  display: flex;
  position: absolute;
  top: 173px;
  left: 283px;
  align-items: flex-start;
  flex-direction: row;
  justify-content: center;
}

.mod .iconPlay {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 42px;
  height: 29px;
}

.mod .iconPlay1 {
  position: relative;
  width: 42px;
  height: 29px;
}

.mod .captionWrapperItem0 {
  box-sizing: border-box;
  display: flex;
  position: absolute;
  top: 144px;
  left: 293px;
  align-items: center;
  flex-direction: row;
  background-size: contain;
  background-image: url(~/assets/government/img_22.png);
  padding-right: 21px;
  padding-left: 20px;
  height: 44px;
  line-height: 30px;
  white-space: nowrap;
}

.mod .caption2 {
  color: #ffffff;
  font-size: 30px;
  font-weight: 400;
}

.mod .wrapper1 {
  display: flex;
  position: absolute;
  top: 200px;
  right: 285px;
  align-items: flex-start;
  flex-direction: column;
  background-size: contain;
  background-color: rgba(215, 245, 109, 0.1);;
  width: 1330px;
  height: 595px;
  line-height: 60px;
  white-space: nowrap;
}

.mod .group {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  margin-top: 78px;
  margin-left: 8px;
  line-height: normal;
  white-space: normal;
}

.mod .longBgWrapperItem0 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  margin-right: 59px;
  width: 623px;
  height: 130px;
}

.mod .longBg {
  position: absolute;
  top: -17px;
  left: 0px;
  width: 623px;
  height: 130px;
  background: rgba(238, 187, 77, 0.55);
  border-radius: 9px;
}

.mod .title3 {
  position: relative;
  margin-top: -1px;
  margin-left: 47px;
  max-width: 529px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 64px;
  white-space: pre;
  color: #184d47;
  font-size: 64px;
  font-weight: 400;
}

.mod .longBgWrapperItem1 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  width: 641px;
  height: 130px;
}

.mod .bar {
  position: absolute;
  top: -16px;
  left: 0px;
  width: 641px;
  height: 130px;
  background: rgba(238, 187, 77, 0.55);
  border-radius: 9px;
}

.mod .caption3 {
  position: relative;
  margin-top: -1px;
  max-width: 629px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 64px;
  white-space: pre;
  color: #184d47;
  font-size: 64px;
  font-weight: 400;
}

.mod .slider {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
  margin-top: 45px;
  margin-left: 8px;
  background-size: contain;
  background: rgba(215, 245, 109, 0.38);
  border-radius: 9px;
  width: 1323px;
  height: 360px;
}

.mod .pointer {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 1323px;
  height: 360px;
  z-index: 1;

}

.mod .summary {
  color: #184d47;
  font-size: 30px;
  font-weight: 400;
  text-overflow: ellipsis;
}


.mod .iconPlay2 {
  position: relative;
  margin-top: 659px;
  margin-left: 283px;
  width: 42px;
  height: 29px;
}

.mod .captionWrapperItem1 {
  box-sizing: border-box;
  display: flex;
  position: absolute;
  top: 818px;
  left: 293px;
  align-items: center;
  flex-direction: row;
  background-size: contain;
  background-image: url(~/assets/government/img_25.png);
  padding-right: 21px;
  padding-left: 20px;
  height: 44px;
  line-height: 30px;
  white-space: nowrap;
}

.mod .caption7 {
  color: #ffffff;
  font-size: 30px;
  font-weight: 400;
}

.mod .wrapper2 {
  display: flex;
  position: absolute;
  top: 860px;
  right: 277px;
  align-items: flex-end;
  flex-direction: row;
  line-height: 46px;
  white-space: nowrap;
}

.mod .layer {
  position: relative;
  width: 1330px;
  height: 1220px;
  line-height: normal;
  white-space: normal;
  background: rgba(215, 245, 109, 0.1);
}


.mod .choose1 {
  position: absolute;
  top: 60px;
  left: 0px;
  width: 1323px;
  height: 650px;
  z-index: 1;

}

.mod .photo1 {
  width: 224px;
  height: 404px;
  border-radius: 15px;
}

.mod .text1 {
  position: absolute;
  left: 80px;
  top: 420px;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
  transform: rotate(-7.74deg);

}

.mod .outer1 {
  position: absolute;
  left: 30px;
  width: 224px;
  height: 404px;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 15px;
  transform: rotate(7.74deg);
}

.mod .outer2 {
  position: absolute;
  left: 380px;
  width: 224px;
  height: 404px;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 15px;
  transform: rotate(7.74deg);
}

.mod .outer3 {
  position: absolute;
  right: 380px;
  width: 224px;
  height: 404px;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 15px;
  transform: rotate(7.74deg);
}

.mod .outer4 {
  position: absolute;
  right: 40px;
  width: 224px;
  height: 404px;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 15px;
  transform: rotate(7.74deg);
}

.mod .choose2 {
  position: absolute;
  top: 730px;
  left: 0px;
  width: 1323px;
  height: 480px;
  z-index: 1;

}

.mod .out1 {
  position: absolute;
  left: 30px;
  width: 220px;
  height: 220px;
  border-radius: 110px;
  background-color: rgba(0, 0, 0, 0.5);
}

.mod .out2 {
  position: absolute;
  left: 380px;
  width: 220px;
  height: 220px;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 220px;
}

.mod .out3 {
  position: absolute;
  right: 380px;
  width: 220px;
  height: 220px;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 110px;
}

.mod .out4 {
  position: absolute;
  right: 60px;
  width: 220px;
  height: 220px;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 110px;
}

.mod .photo2 {
  width: 220px;
  height: 220px;
  border-radius: 110px;
}

.mod .text2 {
  position: absolute;
  height: 40px;
  width: 200px;
  left: 5px;
  top: 240px;
  color: #184d47;
  font-size: 40px;
  font-weight: 400;
  text-align: center;
}

.choose1 /deep/ .el-carousel__container {
  height: 620px;
}

.choose2 /deep/ .el-carousel__container {
  height: 480px;
}

/*// 指示器按钮*/
/deep/ .el-carousel__button {
  width: 25px;
  height: 25px;
  margin-left: 10px;
  margin-right: 7px;
  border: 3px solid rgb(246, 190, 80);
  border-radius: 50%;
  background-color: rgba(196, 196, 196, 0);
}

/*// 指示器激活按钮*/
/deep/ .is-active .el-carousel__button {
  background: rgb(246, 190, 80);
}

</style>
