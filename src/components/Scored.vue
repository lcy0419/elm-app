<template>
  <div class="scored">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/My">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">我的积分</span>
      </div>
      <!-- header-top-end -->

      <!-- header-body -->
      <div class="header-body clear">
        <div class="body-content">
          <div class="body-content-header clear">
            <span class="left">当前积分</span>
            <span class="right">
              <span class="photo">
                <img src="../assets/问号.png" alt />
              </span>
              <router-link to="/ScoredStatement">
                <span>积分说明</span>
              </router-link>
            </span>
          </div>
          <div class="body-content-bory">
            <span>0</span>
            <span>分</span>
          </div>
          <div class="body-content-footer">
            <span @click="change1">积分兑换商品</span>
          </div>
        </div>
      </div>
      <!-- header-body-end -->
    </div>
    <!-- header-end -->

    <!-- body -->
    <div class="content">
      <div class="item1">
        <span>最近30天积分记录</span>
      </div>
      <div class="item2">
        <p>
          <img src="../assets/下载.png" alt />
        </p>
        <p>最近30天无积分记录</p>
        <p>快去下单赚取大量积分吧</p>
      </div>
    </div>
    <!-- body-end -->

    <!-- 弹窗 -->
    <div class="popub" v-show="ended">
      <div class="popub-header">
        <img src="../assets/感叹号.png" alt />
        <p>快去下单赚取大量积分吧</p>
      </div>
      <div class="popub-footer">
        <p @click="change2">确认</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Scored",
  data() {
    return {
      ended: false
    };
  },
  methods: {
    change1() {
      this.ended = true;
    },
    change2() {
      this.ended = false;
    }
  }
};
</script>


<style scoped>
.header-top {
  background-color: #3190e8;
  position: fixed;
  z-index: 100;
  left: 0;
  top: 0;
  width: 100%;
  height: 1.95rem;
}
.header-top span {
  color: #ffffff;
}
.zuo {
  position: relative;
  text-align: center;
  top: 0.3rem;
  left: 1rem;
}
.you {
  position: relative;
  font-size: 0.8rem;
  text-align: center;
  font-weight: 700;
  top: 0.2rem;
  left: 6rem;
}
.header-body {
  border-top: 1px solid #f1f1f11c;
  top: 1.95rem;
  position: relative;
  padding: 0.3rem;
  background-color: #3190e8;
}
.body-content {
  padding: 0.4rem;
  background-color: #fff;
  border-radius: 0.15rem;
}
.body-content-header span {
  font-size: 0.55rem;
}
.body-content-header span:nth-child(1) {
  color: #666;
}
.body-content-header span:nth-child(2) {
  color: #3190e8;
}
.photo {
  position: relative;
  top: 0.1rem;
}
.photo img {
  width: 0.6rem;
  height: 0.6rem;
  margin-right: 0.2rem;
}
.body-content-bory span:nth-child(1) {
  font-size: 1.8rem;
  color: #333;
}
.body-content-bory span:nth-child(2) {
  font-size: 0.7rem;
  color: #333;
  margin-left: 0.31rem;
}
.body-content-footer {
  width: 100%;
  height: 2rem;
  font-size: 0.8rem;

  border-radius: 0.15rem;
  line-height: 2rem;
  margin-top: 1rem;
  text-align: center;
  background-color: #fe6d47;
}
.body-content-footer span {
  color: #fff;
}
.content {
  position: relative;
  top: 1.9rem;
}
.item1 {
  font-size: 0.6rem;
  line-height: 2rem;
  padding-left: 0.5rem;
}
.item1 span {
  color: #999;
}
.item2 {
  text-align: center;
  margin-top: 1rem;
}
.item2 p img {
  width: 8rem;
  height: 5rem;
}
.item2 p:nth-child(2) {
  margin-top: 0.5rem;
  font-size: 0.7rem;
  color: #666;
}
.item2 p:nth-child(3) {
  font-size: 0.5rem;
  color: #999;
}
.popub {
  display: flex;
  flex-direction: column;
  position: absolute;
  top: 50%;
  left: 50%;
  margin-top: -6rem;
  margin-left: -6rem;
  width: 12rem;
  animation: tipMove 0.4s;
  background-color: #fff;
  padding-top: 0.6rem;
  border: 1px;
  border-radius: 0.25rem;
}
.popub-header img {
  position: relative;
  width: 3rem;
  height: 3rem;
  border-radius: 50%;
  top: 0.5rem;
  left: 4.5rem;
}
.popub-header p {
  font-size: 0.7rem;
  color: #333;
  line-height: 0.9rem;
  text-align: center;
  margin-top: 0.8rem;
  padding: 0 0.4rem;
}
.popub-footer {
  font-size: 0.8rem;

  font-weight: 700;
  margin-top: 0.8rem;
  background-color: #4cd964;
  width: 100%;
  text-align: center;
  line-height: 1.8rem;
  border: 1px;
  border-bottom-left-radius: 0.25rem;
  border-bottom-right-radius: 0.25rem;
}
.popub-footer p {
  color: #fff;
}
</style>
