<template>
  <div id="app">
    <div class="tab-top">
      <div class="tab-box">
        <img class="huaweilogo" src="./assets/huawei-logo.png" alt />
        <ul :class="active">
          <li @click="navto" class="banner" :data-to="'banner'">首页</li>
          <li @click="navto" class="daohang" :data-to="'daohang'">新人导航计划</li>
          <li @click="navto" class="xiaoshou" :data-to="'xiaoshou'">销售微场景认证</li>
        </ul>
      </div>
    </div>
    <Banner id="banner"></Banner>
    <Daohang id="daohang"></Daohang>
    <Xiaoshou id="xiaoshou"></Xiaoshou>
    <Footer></Footer>
    <Floating></Floating>
    <!-- <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about"> | About</router-link>
    </div>
    <router-view/>-->
  </div>
</template>
<script>
import Banner from "./components/Banner.vue";
import Daohang from "./components/Daohang";
import Xiaoshou from "./components/Xiaoshou";
import Footer from "./components/footer";
import Floating from "./components/Floating";
import $ from "jquery";

export default {
  name: "app",
  data() {
    return {
      active: "banner"
    };
  },
  components: {
    Banner,
    Daohang,
    Xiaoshou,
    Footer,
    Floating
  },
  methods: {
    navto(e) {
      const id = $(e.target).data("to");
      const topoff = $(".tab-top").height();
      this.active = id;
      $("html").animate({ scrollTop: $("#" + id).offset().top - topoff }, 400);
    }
  }
};
</script>
<style lang="scss">
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  width: 100%;
  position: relative;
}
#banner {
  margin-top: 80px;
}
.huaweilogo {
  position: absolute;
  left: 0;
  width: 135px;
  top: 0;
  bottom: 0;
  margin: auto;
}
.tab-top {
  width: 100%;
  height: 80px;
  line-height: 80px;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 2;
  background-color: #ffffff;
  font-size: 18px;
  color: #000000;
}
.tab-box {
  max-width: 1200px;
  margin: 0 auto;
  position: relative;
}
ul {
  text-align: right;
}
li {
  list-style: none;
  display: inline-block;
  margin-left: 20px;
  cursor: pointer;
  position: relative;
}
ul.banner .banner,
ul.daohang .daohang,
ul.xiaoshou .xiaoshou {
  color: #c7000b;
}
ul.banner .banner::after,
ul.daohang .daohang::after,
ul.xiaoshou .xiaoshou::after {
  content: "";
  position: absolute;
  width: 100%;
  height: 2px;
  background-color: #c7000b;
  left: 0;
  bottom: 15px;
}
@media screen and (max-width: 768px) {
  .huaweilogo {
    width: 1.5rem;
  }
  #banner {
    margin-top: 0.8rem;
  }
  .tab-top {
    height: 0.8rem;
    line-height: 0.8rem;
    font-size: 0.18rem;
    padding: 0 0.3rem;
    box-sizing: border-box;
  }
  ul.banner .banner::after,
  ul.daohang .daohang::after,
  ul.xiaoshou .xiaoshou::after {
    bottom: 0.15rem;
  }
}
</style>
