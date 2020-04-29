<!--  -->
<template>
  <div class="daohang">
    <Title :title="title" :content="content"></Title>
    <div class="daohang-content">
      <div class="daohang-show">
        <div class="daohang-width" v-for="item in lists" :key="item.title">
          <div class="danhang-box">
            <img class="daohang-img" :src="item.img" alt />
            <div class="daohang-title">{{ item.title}}</div>
            <div class="daohang-text">{{ item.text }}</div>
            <div class="know-more">了解更多 →</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.daohang {
  background-color: #e8eff6;
  padding-top: 50px;
  padding-bottom: 80px;
}
.daohang-content {
  font-size: 0;
  max-width: 1200px;
  margin: 0 auto;
  margin-top: 80px;
}
.daohang-show {
  margin-left: -15px;
  margin-right: -15px;
}
.daohang-width {
  width: 25%;
  padding: 0 15px;
  box-sizing: border-box;
  display: inline-block;
}
.danhang-box {
  width: 100%;
  background-color: #ffffff;
  padding: 10px;
  border-radius: 10px;
  box-shadow: 0 2px #c0d0e0;
  box-sizing: border-box;
}
.daohang-img {
  width: 100%;
}
.daohang-title {
  color: #333333;
  font-size: 20px;
  margin-top: 30px;
  margin-bottom: 50px;
  position: relative;
  font-weight: bold;
}
.daohang-title::after {
  content: "";
  position: absolute;
  left: 0;
  right: 0;
  margin: 0 auto;
  width: 50px;
  height: 2px;
  background-color: #cdd1d6;
  bottom: -20px;
}
.daohang-text {
  font-size: 14px;
  color: #666666;
  line-height: 24px;
  padding: 0 15px;
  display: -webkit-box;
  text-overflow: ellipsis;
  overflow: hidden;
  -webkit-line-clamp: 4;
  -webkit-box-orient: vertical;
  height: 96px;
}
.know-more {
  font-size: 14px;
  color: #c7000b;
  font-weight: bold;
  margin-top: 30px;
  margin-bottom: 40px;
}
/* hover */
.danhang-box:hover {
  box-shadow: 0 4px #4c78b5;
}
.danhang-box:hover .daohang-title {
  color: #4c78b5;
}
.danhang-box:hover .daohang-title::after {
  background-color: #4c78b5;
}
.danhang-box:hover .daohang-text {
  color: #4c78b5;
}
.danhang-box:hover .know-more {
  color: #4c78b5;
}
@media screen and (max-width: 768px) {
  .daohang {
    background-color: #e8eff6;
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
  }
  .daohang-content {
    margin-top: 0;
    padding: 0 0.3rem;
  }
  .daohang-width {
    width: 50%;
    padding: 0 0.15rem;
    margin-bottom: 0.3rem;
  }
  .daohang-show {
    margin-left: -0.15rem;
    margin-right: -0.15rem;
  }
  .danhang-box {
    padding: 0.1rem;
  }
  .daohang-title {
    font-size: 0.24rem;
    margin-top: 0.3rem;
    margin-bottom: 0.5rem;
    position: relative;
  }
  .daohang-title::after {
    width: 0.5rem;
    bottom: -0.2rem;
  }
  .daohang-text {
    font-size: 0.18rem;
    color: #666666;
    line-height: 0.35rem;
    padding: 0 0.2rem;
    display: -webkit-box;
    text-overflow: ellipsis;
    overflow: hidden;
    -webkit-line-clamp: 4;
    -webkit-box-orient: vertical;
    height: 1.4rem;
  }
  .know-more {
    font-size: 0.18rem;
    color: #c7000b;
    font-weight: bold;
    margin-top: 0.3rem;
    margin-bottom: 0.2rem;
  }
}
</style>
<script>
import Title from "./../components/title";
export default {
  data() {
    return {
      title: "新人导航计划",
      content:
        "教育行业销售微场景初级认证(HCS-Sale-Education Specialist)是针对生态合作伙伴销售岗位技能要求而设计和开发注重生态合作伙伴面向客户拜访的沟通技巧，销售项目运作等能力的培养，通过学习和测试能够帮助合作伙伴销售人员更好地掌握教育行业销售的技能和方法。通过华为教育行业销售微场景初级认证(HCS-Sale-Education Specialist)，将证明您已经掌握教育行业的客户拜访的沟通方法，销售项目运作知识、行业及产品知识。 当前该课程仅对中国区具备关联公司的华为注册级及以上的生态合作伙伴开放。如您的账号尚未关联华为合作伙伴公司，请登录华为官方网站，在“个人中心-权限管理”中进行关联。",
      lists: [
        {
          img: require("../assets/daohang-img1.png"),
          title: "销售基础",
          text:
            "教育行业销售微场景初级认证(HCS-Sale-Education Specialist )是针对生态合作伙伴销售岗位技能要求而设计和开发注重生态合作伙伴面向客户拜"
        },
        {
          img: require("../assets/daohang-img2.png"),
          title: "产品基础",
          text:
            "教育行业销售微场景初级认证(HCS-Sale-Education Specialist )是针对生态合作伙伴销售岗位技能要求而设计和开发注重生态合作伙伴面向客户拜"
        },
        {
          img: require("../assets/daohang-img3.png"),
          title: "我与华为",
          text:
            "教育行业销售微场景初级认证(HCS-Sale-Education Specialist )是针对生态合作伙伴销售岗位技能要求而设计和开发注重生态合作伙伴面向客户拜"
        },
        {
          img: require("../assets/daohang-img4.png"),
          title: "新人手册",
          text:
            "教育行业销售微场景初级认证(HCS-Sale-Education Specialist )是针对生态合作伙伴销售岗位技能要求而设计和开发注重生态合作伙伴面向客户拜"
        }
      ]
    };
  },
  components: {
    Title
  }
};
</script>
