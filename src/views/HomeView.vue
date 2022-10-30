<template>
  <div class="home">
    <div class="box">
      <!-- 头部 -->
      <div class="header">
        <a href="">实习</a>
        <a href="">求职发布</a>
        <li><img src="../../src/assets/sousuo.jpg" alt="" /></li>
      </div>
      <div class="header1"></div>
      <!-- 中间部分 -->
      <div class="middle">
        <ul>
          <li><a href="">综合</a></li>
          <li><a href="">产品经理</a></li>
          <li><a href="">算法工程师</a></li>
          <img src="../../src/assets/jiahao.jpg" alt="" />
        </ul>
        <ul>
          <li><a href="">推荐</a></li>
          <li><a href="">附近</a></li>
          <li><a href="">最新</a></li>
          <li class="RightText"><a href="">筛选</a></li>
          <li class="RightText"><a href="">上海 </a></li>
        </ul>
      </div>
      <!-- 内容 -->
      <div class="cen" v-for="(item, index) in list" :key="index">
        <ul class="cen1">
          <li>{{ item.name }}</li>
          <li>{{ item.money }}</li>
        </ul>
        <ul class="cen2">
          <li>{{ item.text }}</li>
          <li>{{ item.texts }}</li>
        </ul>
        <ul class="cen3">
          <li>{{ item.dong }}</li>
          <li>{{ item.creature }}</li>
        </ul>
        <ul class="cen4">
          <li>{{ item.head }}</li>
          <li>{{ item.seer }}</li>
          <li>{{ item.manager }}</li>
          <li>{{ item.center }}</li>
          <li><img src="../../src/assets/shanchu.jpg" alt="" /></li>
          <li></li>
        </ul>
      </div>

    </div>
    <div class="bot">
    </div>
    <div class="bott">
      <img src="../assets/zhiwei.jpg" alt="">
      <img src="../assets/xiaoxi.jpg" alt="">
      <img src="../assets/wode.jpg" alt="">
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      list: [
        {
          name: "产品助理",
          money: "120-150/天",
          text: "需求文档",
          texts: "原图设计",
          dong: "京东",
          creature: "1000-9999人",
          head: "hr头像",
          seer: "王先生",
          manager: "·人事经理",
          center: "北京 海淀区",
        },
        {
          name: "产品助理",
          money: "120-150/天",
          text: "需求文档",
          texts: "原图设计",
          dong: "京东",
          creature: "1000-9999人",
          head: "hr头像",
          seer: "王先生",
          manager: "·人事经理",
          center: "北京 海淀区",
        },
        {
          name: "产品助理",
          money: "120-150/天",
          text: "需求文档",
          texts: "原图设计",
          dong: "京东",
          creature: "1000-9999人",
          head: "hr头像",
          seer: "王先生",
          manager: "·人事经理",
          center: "北京 海淀区",
        },
        {
          name: "产品助理",
          money: "120-150/天",
          text: "需求文档",
          texts: "原图设计",
          dong: "京东",
          creature: "1000-9999人",
          head: "hr头像",
          seer: "王先生",
          manager: "·人事经理",
          center: "北京 海淀区",
        },
      ],
    };
  },
};
</script>
<style lang="less">
/* 头部 */
.header1{
  width: 100%;
  height: 50px;
  background-color: #face91;
}
.header {
  width: 100%;
  height: 50px;
  background-color: #face91;
  position: fixed;
  top: 0;
  z-index: 999;
  a {
    text-decoration: none;
    font-size: 20px;
    font-weight: 900;
    color: rgb(0, 0, 0);
    line-height: 50px;
    margin-left: 40px;
  }
  li {
    list-style: none;
    img {
      float: right;
      width: 50px;
      height: 40px;
      margin-top: -45px;
      margin-right: 20px;
    }
  }
}
/* // 中间部分 */
.middle {
  width: 95%;
  height: 100px;
  margin-left: 8px;
  background-color: rgb(255, 255, 255);
  border-bottom: 2px solid #f2f2f2;
  ul > li {
    display: inline-block;
    margin-left: 20px;
    a {
      text-decoration: none;
      color: #000;
      font-size: 16px;
      font-weight: 600;
      line-height: 54px;
    }
  }
  ul > img {
    width: 35px;
    height: 35px;
    margin-top: 10px;
    float: right;
  }
  ul > .RightText {
    float: right;
    a {
      color: rgb(0, 0, 0);
      background-color: #f1f1f1;
      padding: 2px 4px;
      font-weight: 500;
    }
  }
}
// 内容
.cen {
  width: 85%;
  // background-color: rgb(185, 185, 185);
  margin: 0 auto;
  li {
    list-style: none;
    display: inline-block;
  }
  .cen1 {
    margin-top: 10px;
    li:nth-of-type(1) {
      font-weight: 800;
    }
    li:nth-of-type(2) {
      color: #fcca85;
      font-weight: 500;
      float: right;
    }
  }
  .cen2 {
    margin-top: 10px;
    li {
      background-color: rgb(202, 202, 202);
      padding: 2px 4px;
    }
    li:nth-of-type(2) {
      margin-left: 20px;
    }
  }
  .cen3 {
    margin-top: 20px;
    li {
      font-weight: 800;
    }
    li:nth-of-type(2) {
      margin-left: 10px;
    }
  }
  .cen4 {
    margin-top: 10px;
    margin-bottom: -17px;
    li:nth-of-type(1) {
      width: 36px;
      height: 36px;
      border: 1px solid #000;
      line-height: 36px;
      border-radius: 50%;
      font-size: 1px;
      margin-left: -20px;
    }
    li:nth-of-type(2) {
      font-weight: 800;
      margin-left: 10px;
    }
    li:nth-of-type(3) {
      font-weight: 800;
    }
    li:nth-of-type(4) {
      margin-left: 60px;
    }
    li:nth-of-type(5) {
      img {
        width: 20px;
        height: 20px;
        position: relative;
        top: 5px;
        left: 10px;
      }
    }
    li:nth-of-type(6) {
      position: relative;
      width: 108%;
      height: 5px;
      background-color: rgb(223, 223, 223);
      top: -12px;
      left: -20px;
    }
  }
}
.bot{
  width: 100%;
  height: 50px;
  background-color: rgb(255, 255, 255);
  border-top: 1px solid #000;
}
.bott{
  width: 100%;
  height: 50px;
  background-color: rgb(255, 255, 255);
  border-top: 1px solid #000;
  padding-top: 10px;
  position: fixed;
  bottom: 0;
  img{
    width: 38px;
    height: 50px;
    margin-left: 60px;
  }
}
</style>
