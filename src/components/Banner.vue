<!--  -->
<template>
  <div class="banner">
    <img class="banner-img" src="../assets/banner.png" alt />
    <img class="banner-img-ip" src="../assets/banner-ip.png" alt />
    <div class="banner-content">
      <div class="banner-left">
        <div class="banner-title">销售XXXX（名称）</div>
        <div
          class="banner-text"
        >特殊时期下，华为生态大学将加大伙伴赋能投入，为伙伴提供有力保障，共克时艰。我们将为伙伴提供2020年新产品、新技术、新方案的相关培训，帮助伙伴完成知识迭代；共同推广重点行业解决方案，助力机会点拓展。</div>
      </div>
      <div class="banner-right">
        <img class="banner-right-img" src="../assets/banner-img.png" alt />
      </div>
    </div>
    <div class="banner-bottom">
      <img class="tishi-icon" src="../assets/tishi-icon.png" alt />
      <div class="tishi-text tishi-text-pc">如果你已报名，可点击下方对应模块开始学习；如未报名，请添加右侧小V助手微信获取报名方式。</div>
      <div class="tishi-text tishi-text-ip">
        如果你已报名，可点击下方对应模块开始学习；
        <br />如未报名，请添加右侧小V助手微信获取报名方式。
      </div>
    </div>
  </div>
</template>
<style scoped lang="scss">
.banner {
  position: relative;
  overflow: hidden;
}
.banner-img {
  width: 100%;
  display: block;
}
.banner-img-ip {
  width: 100%;
  display: none;
}
.banner-content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 0;
  width: 1200px;
  margin-top: -40px;
}
.banner-left {
  width: 50%;
  display: inline-block;
  vertical-align: middle;
  padding-right: 50px;
  box-sizing: border-box;
}
.banner-title {
  font-size: 60px;
  color: #ffffff;
  text-align: left;
}
.banner-text {
  font-size: 16px;
  color: #ffffff;
  margin-top: 60px;
  line-height: 28px;
  text-align: left;
}
.banner-right {
  width: 50%;
  display: inline-block;
  vertical-align: middle;
}
.banner-right-img {
  width: 110%;
}
.banner-bottom {
  background-color: #ffffff;
  font-size: 14px;
  height: 40px;
  line-height: 40px;
  color: #666666;
}
.tishi-icon {
  width: 24px;
  vertical-align: middle;
  padding-right: 10px;
}
.tishi-text {
  display: inline-block;
}
.tishi-text-pc {
  display: inline-block;
}
.tishi-text-ip {
  display: none;
}
@media screen and (max-width: 768px) {
  .banner-img {
    display: none;
  }
  .banner-img-ip {
    display: block;
  }
  .banner-content {
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 0;
    width: 100%;
    padding: 0 0.3rem;
    box-sizing: border-box;
        margin-top: -0.4rem;
  }
  .banner-left {
    width: 100%;
    padding-right: 0px;
    box-sizing: border-box;
  }
  .banner-title {
    font-size: 0.6rem;
    text-align: center;
  }
  .banner-text {
    font-size: 0.2rem;
    margin-top: 0.2rem;
    line-height: 0.3rem;
    text-align: left;
  }
  .banner-right {
    width: 100%;
  }
  .banner-right-img {
    width: 80%;
    margin: 0 auto;
    margin-top: 0.3rem;
  }
  .banner-bottom {
    height: 0.8rem;
    line-height: 0.24rem;
    width: 6rem;
    font-size: 0;
    position: relative;
    margin: 0 auto;
  }
  .tishi-icon {
    width: 0.41rem;
    padding-right: 0.1rem;
    position: relative;
    top: 50%;
    transform: translateY(-50%);
        margin-top: -0.1rem;
  }
  .tishi-text {
    width: 5.45rem;
    font-size: 0.18rem;
    vertical-align: middle;
    position: relative;
    top: 50%;
    transform: translateY(-50%);
    text-align: left;
  }
  .tishi-text-pc {
    display: none;
  }
  .tishi-text-ip {
    display: inline-block;
  }
}
</style>


<script>
export default {
  data() {
    return {};
  }
};
</script>