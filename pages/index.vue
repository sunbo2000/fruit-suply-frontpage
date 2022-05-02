<template>
  <div>
    <!-- 幻灯片 开始 -->
    <div style="width: 100%">
      <el-carousel :interval="4000" type="card" height="415px">
        <el-carousel-item v-for="(banner, index) in bannerList" :key="index">
          <h3 class="medium">
            <a target="_blank" :href="banner.linkUrl"
            > <img
              style="width: 736px"
              :src="banner.url"
              :alt="banner.name"
            ></img>
            </a>
          </h3>
        </el-carousel-item>
      </el-carousel>
    </div>
    <hr color="CCFF66"/>
    <!--    人物-->
    <div style="position: relative; margin-top: 30px; left: 200px;width: 1100px;">
      <div style="display: inline-block; margin-right: 28px;">
        <a href="#">
          <img
            style="width: 250px;"
            src="~/assets/img/consumer.png"
          /></a>
      </div>
      <div style="display: inline-block; margin-right: 28px;">
        <a href="#"><img
          style="width: 250px;"
          src="~/assets/img/seller.png"
          alt="经营者"/></a>
      </div>
      <div style="display: inline-block; margin-right: 29px; ">
        <a href="#"><img
          style="width: 250px; "
          src="~/assets/img/government.png"
        /></a>
      </div>
      <div style="display: inline-block; ">
        <a href="#"><img
          style="width: 250px;"
          src="~/assets/img/admin.png"
        /></a>
      </div>
    </div>
    <!--      新品-->
    <div style="position: relative;top: 70px;width: 300px; left: 200px; z-index: 1">
      <p
        style="background-color: rgb(233,106,104); color: aliceblue; width: 170px; height: 50px;text-align: center; font-size: 35px;">
        最新产品</p>
    </div>

    <div
      style="margin-top:40px; position: relative; left: 220px; width: 1080px; background-color: rgb(240,249,239);">

      <div
        style="display: inline-block; position: relative; top: 40px; width: 265px; height: 300px; margin-top: 20px; text-align: center">
        <el-avatar :size="150" :src="require('~/assets/img/watermelon.jpg')"></el-avatar>
        <p style="font-size: 30px; font-family: '楷体', '楷体_GB2312', serif">6.6元</p>
      </div>

      <div
        style="display: inline-block; position: relative; top: 40px; width: 265px; height: 300px; margin-top: 20px; text-align: center">
        <el-avatar :size="150" :src="require('~/assets/img/orange.jpg')"></el-avatar>
        <p style="font-size: 30px; font-family: '楷体', '楷体_GB2312', serif">6元</p>
      </div>

      <div
        style="display: inline-block; position: relative; top: 40px; width: 265px; height: 300px; margin-top: 20px; text-align: center">
        <el-avatar :size="150" :src="require('~/assets/img/strawberry.jpg')"></el-avatar>
        <p style="font-size: 30px; font-family: '楷体', '楷体_GB2312', serif">20元</p>
      </div>

      <div
        style=" display: inline-block; position: relative; top: 40px; width: 265px; height: 300px; margin-top: 20px; text-align: center">
        <el-avatar :size="150" :src="require('~/assets/img/banana.jpg')"></el-avatar>
        <p style="font-size: 30px; font-family: '楷体', '楷体_GB2312', serif">8元</p>
      </div>
    </div>

    <!--    分类-->
    <div style="position: relative; top: 40px; left: 220px; width: 1080px;">
      <div style="display: inline-block; width: 357px;  background-color: rgb(231,219,57);text-align: center;">
        <el-avatar style="position: relative; top: 20px;" :size="180"
                   :src="require('~/assets/img/fruit.jpg')"></el-avatar>
        <p style=" color: aliceblue; position: relative;top: 15px;font-size: 30px;">水果</p>
      </div>
      <div style="display: inline-block;width: 357px;text-align: center; background-color: rgb(174,211,232)">
        <el-avatar style="position: relative; top: 20px;" :size="180"
                   :src="require('~/assets/img/vegetable.jpg')"></el-avatar>
        <p style=" color: aliceblue; position: relative;top: 15px;font-size: 30px;">蔬菜</p>
      </div>
      <div style="display: inline-block;width: 356px;text-align: center; background-color: rgb(103,86,132)">
        <el-avatar style="position: relative; top: 20px;" :size="180"
                   :src="require('~/assets/img/drink.jpg')"></el-avatar>
        <p style=" color: aliceblue; position: relative;top: 15px;font-size: 30px;">其他</p>
      </div>
    </div>

    <!--    评论-->
    <div style="position: relative;top: 70px;width: 300px; left: 200px; z-index: 1">
      <p
        style="background-color: rgb(233,106,104); color: aliceblue; width: 170px; height: 50px;text-align: center; font-size: 35px;">
        买家评论</p>
    </div>


    <div
      style=" position: relative; top:20px; left: 220px; width: 1080px; height: 350px;  background-color: rgb(239,249,240);">
      <el-carousel trigger="click" arrow="never" :interval="4000" height="350px">
        <el-carousel-item v-for="(items,index) in commentList" :key="index">
          <h3 class="medium">
            <div
              style="display: inline-block;  position: relative; top: 40px; width: 265px; height: 300px; margin-top: 20px; text-align: center">
              <div
                style="position:relative; border:1px solid rgb(157,239,52); border-radius:15px; top: -30px; left: 35px; width: 200px;height: 130px; text-align: left;">
                <p
                  style="position: relative; top: -15px;font-size: 19px;color:rgb(157,239,52); font-family: '楷体', '楷体_GB2312', serif; padding: 10px">
                  {{ items[0].content.substring(0, 40) }}</p>
                <p style="display: inline-block" v-if="items[0].content.length > 40">......</p>
              </div>
              <el-avatar style="border:2px solid rgb(157,239,52);" :size="80"
                         :src="items[0].avatar"></el-avatar>
            </div>

            <div
              style="display: inline-block; position: relative; top: 40px; width: 265px; height: 300px; margin-top: 20px; text-align: center">
              <div
                style="position:relative; border:1px solid rgb(157,239,52); border-radius:15px;top: -30px; left: 35px; width: 200px;height: 130px; text-align: left;">
                <p
                  style="position: relative; top: -15px;font-size: 19px;color:rgb(157,239,52); font-family: '楷体', '楷体_GB2312', serif; padding: 10px">
                  {{ items[1].content.substring(0, 40) }}</p>
                <p style="display: inline-block" v-if="items[1].content.length > 40">......</p>
              </div>
              <el-avatar style="border:2px solid rgb(157,239,52);" :size="80"
                         :src="items[1].avatar"></el-avatar>
            </div>

            <div
              style="display: inline-block; position: relative; top: 40px; width: 265px; height: 300px; margin-top: 20px; text-align: center">
              <div
                style="position:relative; border:1px solid rgb(157,239,52); border-radius:15px;top: -30px; left: 35px; width: 200px;height: 130px; text-align: left;">
                <p
                  style="position: relative; top: -15px;font-size: 19px;color:rgb(157,239,52); font-family: '楷体', '楷体_GB2312', serif; padding: 10px">
                  {{ items[2].content.substring(0, 40) }}</p>
                <p style="display: inline-block" v-if="items[2].content.length > 40">......</p>
              </div>
              <el-avatar style="border:2px solid rgb(157,239,52);" :size="80"
                         :src="items[2].avatar"></el-avatar>
            </div>

            <div
              style=" display: inline-block; position: relative; top: 40px; width: 265px; height: 300px; margin-top: 20px; text-align: center">
              <div
                style="position:relative; border:1px solid rgb(157,239,52); border-radius:15px;top: -30px; left: 35px; width: 200px;height: 130px; text-align: left;">
                <p
                  style="position: relative; top: -15px;font-size: 19px;color:rgb(157,239,52); font-family: '楷体', '楷体_GB2312', serif; padding: 10px">
                  {{ items[3].content.substring(0, 40) }}</p>
                <p style="display: inline-block" v-if="items[3].content.length > 40">......</p>
              </div>
              <el-avatar style="border:2px solid rgb(157,239,52);" :size="80"
                         :src="items[3].avatar"></el-avatar>
            </div>
          </h3>
        </el-carousel-item>
      </el-carousel>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      commentList: [
        [{
          avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
          content: '很好吃,爱了爱了'
        },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '物流太快了吧'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/C90W2Vux0dmtQJhHGCUw47yI8ELqj5G9tYQaOV1HGPkUSJhe0HLggWIkvwHz11N4dvvNe3O51uMKA4CiczlZq3Q/132',
            content: '家乡水果的味道'
          },
          {
            avatar: 'https://thirdwx.qlogo.cn/mmopen/vi_32/EsJXOTiakxXib1M0r4FWnXpTWmCEM96ef7SsTEO3BHJttlGMvdyXFRmPYG1qSKDGA22anIrvzRgN3nRNhmEg1R7w/132',
            content: '五星推!!!!!!!'
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
      bannerList: [
        {
          name: '',
          url: 'https://th.wallhaven.cc/small/45/45d7d9.jpg',
          linkUrl: ''
        }, {
          name: '',
          url: 'https://th.wallhaven.cc/small/9m/9mzw28.jpg',
          linkUrl: ''
        }, {
          name: '',
          url: 'https://th.wallhaven.cc/small/0w/0wvy6n.jpg',
          linkUrl: ''
        }
      ]
    }
  },
  layout: 'consumer',
  created() {

  }
}
</script>

<style scoped>
/*// 指示器按钮*/
/deep/ .el-carousel__button {
  width: 20px;
  height: 20px;
  border: 3px solid rgb(157,239,52);
  border-radius: 50%;
  background-color: rgba(239,249,240);
}

/*// 指示器激活按钮*/
/deep/ .is-active .el-carousel__button {
  background: rgb(156,238,50);
}

</style>
