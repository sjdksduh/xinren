<!--  -->
<template>
  <div class="footer">
    <div class="footer-left">版权所有©华为技术有限公司 1998-202</div>
    <div class="footer-right">
      <a href="">法律声明</a> |
      <a href="">隐私政策</a>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>
<style scoped>
a {
  color: #ffffff;
  text-decoration: none;
}
.footer {
  width: 100%;
  height: 120px;
  line-height: 120px;
  background-color: #000000;
  font-size: 0px;
  color: #ffffff;
}
.footer-left {
  font-size: 16px;
  display: inline-block;
  width: 50%;
  text-align: left;
  padding-left: 120px;
  box-sizing: border-box;
}
.footer-right {
  font-size: 16px;
  display: inline-block;
  width: 50%;
  text-align: right;
  padding-right: 120px;
  box-sizing: border-box;
}

@media screen and (max-width: 768px) {
  .footer {
    height: 1.2rem;
    line-height: 1.2rem;
    font-size: 0px;
    color: #ffffff;
  }
  .footer-left {
    font-size: 0.16rem;
    display: inline-block;
    width: 65%;
    text-align: left;
    padding-left: 0.3rem;
    box-sizing: border-box;
  }
  .footer-right {
    font-size: 0.16rem;
    display: inline-block;
    width: 35%;
    text-align: right;
    padding-right: 0.3rem;
    box-sizing: border-box;
  }
}
</style>