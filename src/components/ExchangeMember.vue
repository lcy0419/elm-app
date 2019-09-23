<template>
  <div class="member-center">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/MenberCenter">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">兑换会员</span>
      </div>
      <!-- header-top-end -->

      <!-- header-body -->
      <div class="header-body">
        <p>
          成功兑换后将关联到账户
          <span>1169337554</span>
        </p>
      </div>
      <!-- header-body-end -->
    </div>
    <!-- header-end -->

    <!-- body -->
    <form class="item">
      <div class="item1">
        <input type="text" maxlength="10" placeholder="请输入10位卡号" @keyup="present" />
      </div>
      <div class="item2">
        <input type="text" maxlength="6" placeholder="请输入6位卡密" @keyup="present" />
      </div>
    </form>
    <p class="exchange" @click="change">兑换</p>
    <div class="tip">
      <h3>——温馨提示——</h3>
      <p>新兑换的会员服务，权益以「会员说明」为准。</p>
      <p>月卡：30次减免配送费。</p>
      <p>季卡：90次减免配送费。</p>
      <p>年卡：360次减免配送费</p>
      <p>＊仅限蜂鸟专送订单，每日最多减免3单，每单最高减免4元（一个月按31天计算）</p>
    </div>
    <!-- body-end -->

    <!-- 弹窗 -->
    <div class="popub" v-show="this.ended">
      <div class="popub-header">
        <img src="../assets/感叹号.png" alt />
        <p>无效卡号</p>
      </div>
      <div class="popub-footer">
        <p @click="change">确认</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MemberCenter",
  data() {
    return {
      ended: false
    };
  },
  created() {
    this.getUser();
  },

  methods: {
    getUser() {
      this.$axios.get("https://elm.cangdu.org/v1/user").then(res => {
        // console.log(res.data);
      });
    },
    change() {
      this.ended = !this.ended;
    },
    present() {
      var item2Ele = document
        .getElementsByClassName("item2")[0]
        .getElementsByTagName("input")[0];
      var item1Ele = document
        .getElementsByClassName("item1")[0]
        .getElementsByTagName("input")[0];
      var exchangeEle = document.getElementsByClassName("exchange")[0];
      // console.log(exchangeEle);
      if (item1Ele.value.length >= 9 && item2Ele.value.length >= 5) {
        exchangeEle.style.background = "#4cd964";
        // console.log(2);
      }
      if (item1Ele.value.length < 10 || item2Ele.value.length < 6) {
        exchangeEle.style.background = "#ccc";
      }
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
  position: relative;
  top: 2rem;
}
.header-body p {
  font-size: 0.6rem;
  color: #666;
  line-height: 2rem;
  padding-left: 0.7rem;
}
.header-body span {
  font-weight: 700;
  padding-right: 0.3125rem;
}
form {
  margin-top: 0em;
}
.item {
  margin-top: 2rem;
  display: flex;
  flex-direction: column;
}
.item1 input {
  border-bottom: 1px solid #f5f5f5;
  height: 2rem;
  font-size: 0.65rem;
  color: #999;
  padding-left: 0.7rem;
  width: 23rem;
}
.item2 input {
  border-bottom: 1px solid #f5f5f5;
  height: 2rem;
  font-size: 0.65rem;
  color: #999;
  padding-left: 0.7rem;
  width: 23rem;
}
.exchange {
  background-color: #ccc;
  font-size: 0.7rem;
  color: #fff;
  text-align: center;
  margin: 0 0.7rem;
  line-height: 1.8rem;
  border-radius: 0.2rem;
  margin-top: 0.7rem;
  font-weight: 700;
}
h3 {
  text-align: center;
  font-weight: 400;
  font-size: 0.65rem;
  color: #aaa;
  margin-bottom: 0.6rem;
  margin-top: 2rem;
}
.tip p {
  font-size: 0.5rem;
  color: #aaa;
  line-height: 0.8rem;
  padding-left: 2.3rem;
  padding-right: 0.2rem;
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
