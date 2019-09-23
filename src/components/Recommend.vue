<template>
  <div class="member-center">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/Discount">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">推荐有奖</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->

    <!-- body -->
    <div class="content">
      <div class="item1">
        <img src="../assets/activity.png" alt />
      </div>
      <div class="item2">
        <div @click="change1">
          <img src="../assets/webchat.png" alt />
          <p>邀请微信好友</p>
        </div>
        <div @click="change1">
          <img src="../assets/QQ.png" alt />
          <p>邀请QQ好友</p>
        </div>
        <div @click="change1">
          <img src="../assets/chat.png" alt />
          <p>面对面邀请</p>
        </div>
      </div>
      <div class="item3">
        <div>
          <p>累计收益</p>
          <p>
            <span>0</span>元
          </p>
        </div>
        <div></div>
        <div>
          <p>成功邀请</p>
          <p>
            <span>0</span>人
          </p>
        </div>
      </div>
      <div class="item4">
        <p>-收益明细-</p>
        <p>
          <img src="../assets/money.png" alt />
        </p>
        <p>还不赶紧去邀请好友</p>
      </div>
    </div>
    <!-- body-end -->

    <!-- 弹窗 -->
    <div class="popub" v-show="ended">
      <div class="popub-header">
        <img src="../assets/感叹号.png" alt />
        <p>请在饿了么APP中打开</p>
      </div>
      <div class="popub-footer">
        <p @click="change2">确认</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Recommend",
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
  border-bottom: 1px solid rgba(255, 255, 255, 0.205);
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
.content {
  margin-top: 1.9rem;
}
.content img {
  width: 100%;
  height: 10rem;
}
.item2 {
  margin-top: 0.1rem;
  display: flex;
  justify-content: space-around;
  background: #fff;
  padding-top: 1rem;
  padding-bottom: 1rem;
}
.item2 img {
  width: 2.5rem;
  height: 2.5rem;
}
.item2 p {
  font-size: 0.5rem;
  color: #333;
}
.item3 {
  display: flex;
  justify-content: space-around;
  margin-top: 1rem;
  margin-left: 1rem;
  margin-right: 1rem;
}

.item3 p {
  font-size: 0.5rem;
  color: #666;
  text-align: center;
}
.item3 div:nth-child(2) {
  border-right: 1px solid #ddd;
}
.item3 div:nth-child(1) span {
  font-size: 0.8rem;
  color: #ff5633;
  font-weight: 700;
}
.item3 div:nth-child(3) span {
  font-size: 0.8rem;
  color: #666;
  font-weight: 700;
}
.item4 p {
  text-align: center;
  margin-top: 1rem;
}
.item4 p:nth-child(1) {
  font-size: 0.5rem;
  color: #666;
}
.item4 p:nth-child(2) img {
  width: 1.3rem;
  height: 1.6rem;
}
.item4 p:nth-child(3) {
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
