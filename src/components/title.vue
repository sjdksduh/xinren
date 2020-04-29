<!--  -->
<template>
  <div class="title-box">
    <div class="title">{{ title }}</div>
    <div class="contenttext">{{ content }}</div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    content: String
    // required: true
  },
  data() {
    return {
      // title: "新人导航计划",
      // content:
      //   "教育行业销售微场景初级认证(HCS-Sale-Education Specialist)是针对生态合作伙伴销售岗位技能要求而设计和开发注重生态合作伙伴面向客户拜访的沟通技巧，销售项目运作等能力的培养，通过学习和测试能够帮助合作伙伴销售人员更好地掌握教育行业销售的技能和方法。通过华为教育行业销售微场景初级认证(HCS-Sale-Education Specialist)，将证明您已经掌握教育行业的客户拜访的沟通方法，销售项目运作知识、行业及产品知识。 当前该课程仅对中国区具备关联公司的华为注册级及以上的生态合作伙伴开放。如您的账号尚未关联华为合作伙伴公司，请登录华为官方网站，在“个人中心-权限管理”中进行关联。"
    };
  }
};
</script>
<style scoped>
.title-box {
  max-width: 1200px;
  margin: 0 auto;
  text-align: left;
}
.title {
  font-size: 40px;
  color: #333333;
  font-weight: bold;
  text-align: center;
}
.contenttext {
  font-size: 16px;
  color: #666666;
  line-height: 28px;
  margin-top: 30px;
  position: relative;
  margin-bottom: 30px;
}
.contenttext::after {
  content: "";
  position: absolute;
  left: 0;
  right: 0;
  margin: 0 auto;
  width: 80px;
  height: 4px;
  background-color: #cdd1d6;
  bottom: -30px;
}
@media screen and (max-width: 768px) {
  .title {
    font-size: 0.4rem;
  }
  .contenttext {
    font-size: 0.18rem;
    line-height: 0.4rem;
    padding: 0 0.3rem;
    margin-top: 0.6rem;
    margin-bottom: 0.6rem;
  }
  .contenttext::after {
    width: 0.8rem;
    height: 4px;
    top: -0.3rem;
  }
}
</style>