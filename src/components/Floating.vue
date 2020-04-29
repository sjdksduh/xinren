<!--  -->
<template>
  <div class="floating">
    <img class="er-icon" src="../assets/er-icon.png" alt />
    <div class="floating-text">
      扫码添加小V助手
      <br />获取报名方式
    </div>
  </div>
</template>
<style scoped>
.floating {
  position: fixed;
  top: 50%;
  transform: translateY(-50%);
  right: 40px;
  background-color: #c7000b;
  border-radius: 10px;
  padding: 20px 10px 15px;
}
.er-icon {
  width: 78px;
  margin: 0 auto;
  display: block;
}
.floating-text {
  font-size: 14px;
  color: #ffffff;
  margin-top: 15px;
}
@media screen and (max-width: 768px) {
  .floating {
    position: fixed;
    top: 50%;
    transform: translateY(-50%);
    right: 0.1rem;
    background-color: #c7000b;
    border-radius: 0.1rem;
    padding: 0.4rem 0.1rem 0.3rem;
  }
  .er-icon {
    width: 0.78rem;
    margin: 0 auto;
    display: block;
  }
  .floating-text {
    font-size: 0.14rem;
    margin-top: 0.2rem;
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
