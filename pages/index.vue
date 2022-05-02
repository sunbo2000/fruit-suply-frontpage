<template>
  <div>
    <!-- 幻灯片 开始 -->
    <div style="width: 100%">
      <el-carousel :interval="4000" type="card" trigger="click" height="415px">
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
        /></a>
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
    <div
      style="margin-top:40px; position: relative; left: 200px; width: 1100px; background-color: rgb(240,249,239);">
      <div style="position: relative; top: 40px; width: 300px; height: 300px; margin-top: 20px; text-align: center">
        <el-avatar :size="150" :src="require('~/assets/img/banana.jpg')"></el-avatar>
        <p style="font-size: 30px">5 元</p>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
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
    console.log("fjadskjfkldsjfdklsfj++++++++++++++++++++++++++++++++++++++++++")
  }
}
</script>
