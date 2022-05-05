<template>
  <!--  在这里写html,vue前端代码-->
  <el-main class="main1">
    <svg-icon class="tip5" icon-class="tip"/>
    <div class="product">
      <div class="div1">
        <!--        <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_3.png')" fit="cover"></el-avatar>-->
        <img class="new1" src="~/assets/img/img_3.png"/>
        <p class="m">猕猴桃</p>
        <p class="price">￥29.9</p>&nbsp;<p class="priceOld">￥39.8</p>
      </div>
      <div class="div1">
        <!--        <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_4.png')" fit="cover" alt="new1"/>-->
        <img class="new1" src="~/assets/img/img_4.png"/>
        <p class="m">苹果</p>
        <p class="price">￥9.8</p>&nbsp;<p class="priceOld">￥19.8</p>
      </div>
      <div class="div1">
        <!--        <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_5.png')" fit="cover" alt="new2"/>-->
        <img class="new1" src="~/assets/img/img_5.png"/>
        <p class="m">橙子</p>
        <p class="price">￥19.8</p>&nbsp;<p class="priceOld">￥29.8</p>
      </div>
      <div class="div1">
        <!--        <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_6.png')" fit="cover" alt="new2"/>-->
        <img class="new1" src="~/assets/img/img_6.png"/>
        <p class="m">车厘子</p>
        <p class="price">￥49.8</p>&nbsp;<p class="priceOld">￥59.8</p>
      </div>
      <div class="div1">
        <!--        <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_8.png')" fit="cover" alt="new2"/>-->
        <img class="new1" src="~/assets/img/img_8.png"/>
        <p class="m">菠萝</p>
        <p class="price">￥29.9</p>&nbsp;<p class="priceOld">￥39.9</p>
      </div>
      <div class="div1">
        <!--        <el-avatar class="new1" :size="size" :src="require('~/assets/img/img_7.png')" fit="cover" alt="new2"/>-->
        <img class="new1" src="~/assets/img/img_7.png"/>
        <p class="m">草莓</p>
        <p class="price">￥39.8</p>&nbsp;<p class="priceOld">￥59.8</p>
      </div>
    </div>
    <!--    -->
    <!--    分类-->
    <div class="div3">
      <div class="p2">
        <img class="p3" src="~/assets/img/img_10.png" alt="s"/>
        <p
          class="fontP">
          时鲜水果</p>
      </div>
      <div class="p2">
        <img class="p3" src="~/assets/img/img_11.png" alt="s"/>
        <p class="fontP">
          进口优果</p>
      </div>
      <div class="p2">
        <img class="p3" src="~/assets/img/img_12.png" alt="s"/>
        <p class="fontP">
          今日团购</p>
      </div>
    </div>

    <svg-icon class="tip6" icon-class="suy"/>
    <div class="square4">
      <div class="p5">
        <img class="img6" src="~/assets/img/img_13.png" alt="s"/>
        <p class="font5">
          产地参观</p>
      </div>
      <div class="p5">
        <img class="img6" src="~/assets/img/img_14.png" alt="s"/>
        <p class="font5">
          生长过程</p>
      </div>
      <div class="p5">
        <img class="img6" src="~/assets/img/img_15.png" alt="s"/>
        <p class="font5">
          实施物流</p>
      </div>
    </div>
    <!--    -->
    <svg-icon class="tip7" icon-class="commentTip"/>
    <div class="banner1">
      <el-carousel arrow="never" :interval="4000">
        <el-carousel-item v-for="(items,index) in commentList" :key="index">
          <h3 class="medium">
            <div
              class="banner2">
              <div class="banner3">
                <svg-icon class="banner4"
                          icon-class="comment"/>
                <p class="comment5">
                  {{ items[0].content }}</p>
                <p style="display: inline-block" v-if="items[0].content.length > 36">......</p>
              </div>
              <img class="avatar1" :src="items[0].avatar"/>
              <p class="nickname">@{{ items[0].name }}</p>
            </div>

            <div
              class="banner2">
              <div class="banner3">
                <svg-icon class="banner4"
                          icon-class="comment"/>
                <p class="comment5">
                  {{ items[1].content }}</p>
                <p style="display: inline-block" v-if="items[1].content.length > 36">......</p>

              </div>
              <img class="avatar1" :src="items[1].avatar"/>
              <p class="nickname">@{{ items[1].name }}</p>
            </div>

            <div
              class="banner2">
              <div class="banner3">
                <svg-icon class="banner4"
                          icon-class="comment"/>
                <p class="comment5">
                  {{ items[2].content }}</p>
                <p style="display: inline-block" v-if="items[2].content.length > 36">......</p>
              </div>
              <img class="avatar1" :src="items[2].avatar"/>
              <p class="nickname">@{{ items[2].name }}</p>
            </div>

            <div
              class="banner2">
              <div class="banner3">
                <svg-icon class="banner4"
                          icon-class="comment"/>
                <p class="comment5">
                  {{ items[3].content }}</p>
                <p style="display: inline-block" v-if="items[3].content.length > 36">......</p>
              </div>
              <img class="avatar1" :src="items[3].avatar"/>
              <p class="nickname">@{{ items[3].name }}</p>
            </div>
          </h3>
        </el-carousel-item>
      </el-carousel>
    </div>
  </el-main>
</template>
<script>
export default {
  data() {
    return {
      size: 140,
      commentList: [
        [{
          avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
          content: '很好吃,爱了爱了',
          name: '用户a'
        },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '物流太快了吧',
            name: '用户9823'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/C90W2Vux0dmtQJhHGCUw47yI8ELqj5G9tYQaOV1HGPkUSJhe0HLggWIkvwHz11N4dvvNe3O51uMKA4CiczlZq3Q/132',
            content: '家乡水果的味道',
            name: '一只小芭蕾'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '五星推!!!!!!!',
            name: '小可爱'
          },
        ],
        [{
          avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
          content: '强烈推荐,一定要尝尝呀,太好吃了',
          name: '熊大'
        },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '没想到会这么快,第一天买的隔天就到了',
            name: '大甲虫'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/C90W2Vux0dmtQJhHGCUw47yI8ELqj5G9tYQaOV1HGPkUSJhe0HLggWIkvwHz11N4dvvNe3O51uMKA4CiczlZq3Q/132',
            content: '水果很新鲜,没有坏掉的,超赞',
            name: '细水长流'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/C90W2Vux0dmtQJhHGCUw47yI8ELqj5G9tYQaOV1HGPkUSJhe0HLggWIkvwHz11N4dvvNe3O51uMKA4CiczlZq3Q/132',
            content: '溯源功能太好用了,很有安全感',
            name: '自由飞翔'
          },
        ],
        [{
          avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
          content: '会回购,推荐给了身边好多人',
          name: '炎龙铠甲'
        },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '超赞的好不好!!!',
            name: '张无忌'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '一定要买呀',
            name: '嘻嘻哈哈'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/9J93ZOHAHknYUibBxgq1rs3VLToDtD0icrQg7MCyTQzBUppD94MZ7evn8FDicf7ic3yHYO62pyAHXscS74IKM6egDw/132',
            content: '直接五星!',
            name: '用户1312'
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
.main1 {
  position: relative;
  width: 100%;
  height: 2404px;
  overflow: hidden;
}

.tag {
  /* 消费者界面 */
  position: absolute;
  width: 271px;
  height: 129.72px;
  top: 0;
  left: 250px;
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

.tip5 {
  /* 提示标 */
  position: absolute;
  width: 171px;
  height: 58px;
  top: 242px;
  left: 282px;
}

.product {
  /* 矩形 8 */
  position: absolute;
  width: 1325px;
  height: 352px;
  top: 253px;
  left: 303px;


  background: rgba(215, 245, 109, 0.05);
}

.new1 {
  width: 170px;
  height: 170px;
  border-radius: 50%;
  position: relative;
  top: 50px;
}

.div1 {
  width: 215px;
  display: inline-block;
  height: 200px;
  text-align: center;
}

.m {
  position: relative;
  height: 30px;
  top: 50px;

  color: rgb(216, 74, 29);
  font-family: 幼圆, serif;
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
  font-size: 15px;
  top: 15px;
  color: rgb(216, 74, 29);
  text-decoration: line-through;
  display: inline-block;
}

.div3 {
  /* 矩形 8 */
  position: absolute;
  width: 1325px;
  height: 352px;
  top: 647px;
  left: 303px;
}

.p2 {
  display: inline-block;
  width: 438px;
  height: 278px;
  text-align: center;
}

.p3 {
  /* 矩形 10 */
  width: 438px;
  height: 278px;
  opacity: 0.7;
}

.fontP {
  z-index: 1;
  position: relative;
  top: -280px;

  color: rgb(255, 255, 255);
  font-family: '楷体', '楷体_GB2312', serif;
  font-size: 96px;
  font-weight: 400;
  line-height: 110px;
  letter-spacing: 0px;

}

.font5 {
  position: relative;
  top: -30px;

  /* 产地参观 */
  width: 300px;
  height: 55px;
  left: 0px;

  color: rgb(24, 77, 71);
  font-family: 幼圆, serif;
  font-size: 48px;
  font-weight: 400;
  line-height: 55px;
  letter-spacing: 20px;
  text-align: left;


}

.square4 {
  /* 矩形 8 */
  position: absolute;
  width: 1325px;
  height: 549px;
  top: 1010px;
  left: 301px;

  background: rgba(215, 245, 109, 0.05);
}

.p5 {
  display: inline-block;
  position: relative;
  width: 438px;
  top: 83px;

}

.img6 {
  width: 438px;
  height: 352px;
}

.tip6 {
  /* 提示标2 */
  position: absolute;
  width: 171px;
  height: 58px;
  top: 988px;
  left: 269px;
}

.tip7 {
  /* 提示标3 */
  position: absolute;
  width: 171px;
  height: 58px;
  top: 1601px;
  left: 269px;
}

.banner1 {
  /* 矩形 8 */
  position: absolute;
  width: 1323px;
  height: 729px;
  top: 1623px;
  left: 303px;


  background: rgba(215, 245, 109, 0.05);
}

.banner2 {
  display: inline-block;
  position: relative;
  top: 94px;
  width: 320px;
  height: 300px;
  margin-top: 20px;
  text-align: center;
}

.banner3 {
  position: relative;
  width: 268.78px;
  height: 179px;
  top: 0px;
  left: 35px;
  text-align: left;
}

.banner4 {
  font-size: 200px;
  position: absolute;
  width: 268.78px;
  top: -50px;
  left: 0px;
}

.comment5 {
  position: relative;
  top: -35px;
  width: 238px;
  height: 179px;
  color: rgb(24, 77, 71);
  font-family: 幼圆, serif;
  padding: 20px;

  font-size: 24px;
  font-weight: 400;
  line-height: 27px;
  letter-spacing: 0px;
  text-align: left;
}

.avatar1 {
  width: 190px;
  height: 190px;
  border-radius: 50%;
  border: 2px solid rgb(157, 239, 52);
}

.nickname {
  /* @用户a */
  position: relative;
  height: 55px;
  left: 0px;
  z-index: 1;

  color: rgb(24, 77, 71);
  font-family: 幼圆, serif;
  font-size: 48px;
  font-weight: 400;
  line-height: 55px;
  letter-spacing: 0px;
  text-align: center;
}

/deep/ .el-carousel__container{
  height: 720px;
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
