<template>
  <!--  在这里写html,vue前端代码-->
  <el-main style="margin: 0; padding: 0; border: 0">
    <div class="web">

      <div class="tag">
        <svg-icon style="font-size: 200px;" icon-class="consumer"/>
      </div>
      <div class="tag1">
        <svg-icon style="font-size: 200px;" icon-class="seller"/>
      </div>
      <div class="tag2">
        <svg-icon style="font-size: 200px;" icon-class="government"/>
      </div>
      <div class="tag3">
        <svg-icon style="font-size: 200px;" icon-class="admin"/>
      </div>

      <svg-icon style="font-size: 200px; position: absolute; top: 130px; left: 160px;" icon-class="tip"/>
      <div class="product">
        <div class="div1">
          <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_3.png')" fit="cover"></el-avatar>
          <p class="m">猕猴桃</p>
          <p class="price">￥29.9</p>&nbsp;<p class="priceOld">￥20</p>
        </div>
        <div class="div1">
          <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_4.png')" fit="cover" alt="new1"/>
          <p class="m">苹果</p>
          <p class="price">￥29.9</p>&nbsp;<p class="priceOld">￥20</p>
        </div>
        <div class="div1">
          <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_5.png')" fit="cover" alt="new2"/>
          <p class="m">"橙子</p>
          <p class="price">￥29.9</p>&nbsp;<p class="priceOld">￥20</p>
        </div>
        <div class="div1">
          <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_6.png')" fit="cover" alt="new2"/>
          <p class="m">车厘子</p>
          <p class="price">￥29.9</p>&nbsp;<p class="priceOld">￥20</p>
        </div>
        <div class="div1">
          <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_8.png')" fit="cover" alt="new2"/>
          <p class="m">菠萝</p>
          <p class="price">￥29.9</p>&nbsp;<p class="priceOld">￥20</p>
        </div>
        <div class="div1">
          <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_7.png')" fit="cover" alt="new2"/>
          <p class="m">草莓</p>
          <p class="price">￥29.9</p>&nbsp;<p class="priceOld">￥20</p>
        </div>
      </div>
      <!--    -->
      <!--    分类-->
      <div style="position: absolute; top:540px; left: 193px; width: 1063px;height: 224px;">
        <div style="display: inline-block; height: 223px; text-align: center;">
          <img style="opacity:0.6; width: 351px;" src="~/assets/img/img_10.png" alt="s"/>
          <p
            style=" color: rgb(255, 255, 255);z-index: 1; position: relative; font-weight: bold; top: -240px;font-size: 85px;font-family: '楷体', '楷体_GB2312', serif">
            时鲜水果</p>
        </div>
        <div style="display: inline-block; height: 223px;text-align: center;">
          <img style="opacity:0.6; width: 351px;" src="~/assets/img/img_11.png" alt="s"/>
          <p
            style=" color: rgb(255, 255, 255);z-index: 1; position: relative; font-weight: bold; top: -240px;font-size: 85px;font-family: '楷体', '楷体_GB2312', serif">
            进口优果</p>
        </div>
        <div style="display: inline-block;height: 223px; text-align: center;">
          <img style="opacity:0.6; width: 351px;" src="~/assets/img/img_12.png" alt="s"/>
          <p
            style=" color: rgb(255, 255, 255); z-index: 1; position: relative; font-weight: bold; top: -240px;font-size: 85px;font-family: '楷体', '楷体_GB2312', serif">
            今日团购</p>
        </div>
      </div>

      <svg-icon style="font-size: 200px; position: absolute; z-index: 1; top: 740px; left: 160px;" icon-class="suy"/>
      <div class="square4">
        <div style="display: inline-block; position: relative; top: 50px;">
          <img style=" width: 351px;" src="~/assets/img/img_13.png" alt="s"/>
          <p class="font5">
            产地参观</p>
        </div>
        <div style="display: inline-block;position: relative; top: 50px;">
          <img style=" width: 351px; height: 293px;" src="~/assets/img/img_14.png" alt="s"/>
          <p class="font5">
            生长过程</p>
        </div>
        <div style="display: inline-block; position: relative; top: 50px;">
          <img style=" width: 351px;" src="~/assets/img/img_15.png" alt="s"/>
          <p class="font5">
            实施物流</p>
        </div>
      </div>
      <!--    -->
      <svg-icon style="font-size: 200px; position: absolute; z-index: 1; top: 1200px; left: 160px;"
                icon-class="commentTip"/>
      <div class="banner1">
        <el-carousel trigger="click" arrow="never" :interval="4000" height="480px">
          <el-carousel-item v-for="(items,index) in commentList" :key="index">
            <h3 class="medium">
              <div
                style="display: inline-block;  position: relative; top: 40px; width: 260px; height: 300px; margin-top: 20px; text-align: center">
                <div
                  style="position:relative;  border-radius:15px; top: -30px; left: 35px; width: 200px;height: 110px; text-align: left;">
                  <svg-icon style="font-size: 200px;  position: absolute;  top: -50px; left: -3px;"
                            icon-class="comment"/>
                  <p
                    style="position: relative; top: -15px; font-size: 19px; width:188px; color:rgb(24, 77, 71); font-family: '方正舒体', serif; padding: 10px">
                    {{ items[0].content }}</p>
                  <p style="display: inline-block" v-if="items[0].content.length > 40">......</p>
                </div>
                <el-avatar style="border:2px solid rgb(157,239,52);" :size="150"
                           :src="items[0].avatar"></el-avatar>
                <p>{{ items[1].name }}</p>
              </div>

              <div
                style="display: inline-block;  position: relative; top: 40px; width: 260px; height: 300px; margin-top: 20px; text-align: center">
                <div
                  style="position:relative;  border-radius:15px; top: -30px; left: 35px; width: 200px;height: 110px; text-align: left;">
                  <svg-icon style="font-size: 200px;  position: absolute;  top: -50px; left: -3px;"
                            icon-class="comment"/>
                  <p
                    style="position: relative; top: -15px; font-size: 19px; width:188px; color:rgb(24, 77, 71); font-family: '方正舒体', serif; padding: 10px">
                    {{ items[1].content }}</p>
                  <p style="display: inline-block" v-if="items[1].content.length > 40">......</p>

                </div>
                <el-avatar style="border:2px solid rgb(157,239,52);" :size="150"
                           :src="items[1].avatar"></el-avatar>
                <p>{{ items[1].name }}</p>
              </div>

              <div
                style="display: inline-block;  position: relative; top: 40px; width: 260px; height: 300px; margin-top: 20px; text-align: center">
                <div
                  style="position:relative;  border-radius:15px; top: -30px; left: 35px; width: 200px;height: 110px; text-align: left;">
                  <svg-icon style="font-size: 200px;  position: absolute;  top: -50px; left: -3px;"
                            icon-class="comment"/>
                  <p
                    style="position: relative; top: -15px; font-size: 19px; width:188px; color:rgb(24, 77, 71); font-family: '方正舒体', serif; padding: 10px">
                    {{ items[2].content }}</p>
                  <p style="display: inline-block" v-if="items[2].content.length > 40">......</p>
                </div>
                <el-avatar style="border:2px solid rgb(157,239,52);" :size="150"
                           :src="items[2].avatar"></el-avatar>
                <p>{{ items[1].name }}</p>
              </div>

              <div
                style="display: inline-block;  position: relative; top: 40px; width: 260px; height: 300px; margin-top: 20px; text-align: center">
                <div
                  style="position:relative;  border-radius:15px; top: -30px; left: 35px; width: 200px;height: 110px; text-align: left;">
                  <svg-icon style="font-size: 200px;  position: absolute;  top: -50px; left: -3px;"
                            icon-class="comment"/>
                  <p
                    style="position: relative; top: -15px; font-size: 19px; width:188px; color:rgb(24, 77, 71); font-family: '方正舒体', serif; padding: 10px">
                    {{ items[3].content }}</p>
                  <p style="display: inline-block" v-if="items[3].content.length > 40">......</p>
                </div>
                <el-avatar style="border:2px solid rgb(157,239,52);" :size="150"
                           :src="items[3].avatar"></el-avatar>
                <p>{{ items[1].name }}</p>
              </div>
            </h3>
          </el-carousel-item>
        </el-carousel>
      </div>
    </div>
  </el-main>
</template>
<script>
export default {
  data() {
    return {
      size: 120,
      commentList: [
        [{
          avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
          content: '很好吃,爱了爱了',
          name: 'qq'
        },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '物流太快了吧',
            name: 'qq'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/C90W2Vux0dmtQJhHGCUw47yI8ELqj5G9tYQaOV1HGPkUSJhe0HLggWIkvwHz11N4dvvNe3O51uMKA4CiczlZq3Q/132',
            content: '家乡水果的味道',
            name: 'qq'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '五星推!!!!!!!',
            name: 'qq'
          },
        ],
        [{
          avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
          content: '强烈推荐,一定要尝尝呀,太好吃了'
        },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '没想到会这么快,第一天买的隔天就到了'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/C90W2Vux0dmtQJhHGCUw47yI8ELqj5G9tYQaOV1HGPkUSJhe0HLggWIkvwHz11N4dvvNe3O51uMKA4CiczlZq3Q/132',
            content: '水果很新鲜,没有坏掉的,超赞'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/C90W2Vux0dmtQJhHGCUw47yI8ELqj5G9tYQaOV1HGPkUSJhe0HLggWIkvwHz11N4dvvNe3O51uMKA4CiczlZq3Q/132',
            content: '溯源功能太好用了,很有安全感'
          },
        ],
        [{
          avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
          content: '会回购,推荐给了身边好多人'
        },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '超赞的好不好!!!'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '一定要买呀'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/9J93ZOHAHknYUibBxgq1rs3VLToDtD0icrQg7MCyTQzBUppD94MZ7evn8FDicf7ic3yHYO62pyAHXscS74IKM6egDw/132',
            content: '直接五星!'
          },
        ]
      ],
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
.web {
  /* web 1920 */
  position: relative;
  height: 1800px;
  left: 200px;
}

.tag {
  /* 消费者界面 */
  position: absolute;
  width: 271px;
  height: 129.72px;
  top: 0;
  left: 192px;
}

.tag1 {
  /* 经营者界面 */
  position: absolute;
  width: 271px;
  height: 86px;
  top: -17px;
  left: 480px;
}

.tag2 {
  /* 政府人员界面 */
  position: absolute;
  width: 271px;
  height: 86px;
  top: -17px;
  left: 770px;
}

.tag3 {
  /* 维护人员界面 */
  position: absolute;
  width: 271px;
  height: 86px;
  top: -17px;
  left: 1057px;

}

.product {
  /* 矩形 8 */
  position: absolute;
  width: 1064px;
  height: 280px;
  top: 230px;
  left: 193px;


  background: rgba(215, 245, 109, 0.05);
}

.new1 {
  position: relative;
  top: 60px;
}

.div1 {
  width: 170px;
  display: inline-block;
  height: 200px;
  text-align: center;
}

.m {
  /* 猕猴桃 */
  position: relative;
  height: 30px;
  top: 50px;

  color: rgb(216, 74, 29);
  font-family: Noto Sans SC, serif;
  font-size: 20px;
  font-weight: 400;
  line-height: 30px;
  letter-spacing: 0px;
}

.price {
  /* ¥29.9 ¥39.9 */
  position: relative;
  font-size: 20px;
  top: 15px;
  color: rgb(216, 74, 29);
  display: inline-block;
}

.priceOld {
  /* ¥29.9 ¥39.9 */
  position: relative;
  font-size: 20px;
  top: 15px;
  color: rgb(216, 74, 29);
  text-decoration: line-through;
  display: inline-block;
}

.font5 {
  position: relative;
  top: -30px;
  color: rgb(24, 77, 71);
  font-family: 幼圆, serif;
  font-size: 38px;
  font-weight: bold;
  line-height: 50px;
  letter-spacing: 16px;
  text-align: left;
}

.square4 {
  /* 矩形 8 */
  position: absolute;
  top: 840px;
  left: 193px;
  width: 1063px;
  height: 450px;

  background: rgba(215, 245, 109, 0.05);
}

.banner1 {
  position: absolute;
  top: 1300px;
  left: 193px;
  width: 1063px;
  height: 480px;
  background-color: rgba(215, 245, 109, 0.05);
}

/*// 指示器按钮*/
/deep/ .el-carousel__button {
  width: 20px;
  height: 20px;
  border: 3px solid rgb(246, 190, 80);
  border-radius: 50%;
  background-color: rgba(196, 196, 196, 0);
}

/*// 指示器激活按钮*/
/deep/ .is-active .el-carousel__button {
  background: rgb(246, 190, 80);
}
</style>
