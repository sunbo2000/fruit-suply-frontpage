<template>
  <!--  在这里写html,vue前端代码-->
  <main class="pbmMain">
    <a href="/consumer" style="text-decoration: none;"><h1 align="center">去消费者那康康--></h1></a>
    <a href="/seller" style="text-decoration: none;"><h1 align="center">去经营者那康康--></h1></a>
    <a href="/admin" style="text-decoration: none;"><h1 align="center">去科技工作者那康康--></h1></a>
    <a href="/government" style="text-decoration: none;"><h1 align="center">去科技政府人员那康康--></h1></a>
  </main>
</template>

<script>
import cookie from "js-cookie";

export default {
  data() {
    return {
      //  数据
    }
  },
  created() {
    this.$router.push({path: '/login'});
  },
  methods: {
    //  编写方法
  }
}

</script>
<style scoped>
.pbmMain {
  position: relative;
  margin: 0;
  padding: 0;
  border: 0;
  width: 100%;
}

/*css 代码*/
.web1 {
  position: relative;
  width: 100%;
  height: 800px;
  left: 0;

  background: rgb(255, 255, 255);
}

.square4 {
  position: absolute;
  width: 100%;
  left: 0;
}

.square5 {
  /* logo无字 1 */
  position: relative;
  width: 560px;
  height: 494px;
  top: 0px;
  left: -12px;
}

.des {
  /* 果宝特供 */
  position: relative;
  width: 415px;
  height: 128px;
  top: 0px;
  left: 61px;


  color: rgb(24, 77, 71);
  font-family: HappyZcool-2016, serif;
  font-size: 100px;
  font-weight: 400;
  line-height: 114px;
  letter-spacing: 0px;
  text-align: left;
}

a {
  color: cadetblue;
}

a:hover {
  color: cornflowerblue;
}
</style>
