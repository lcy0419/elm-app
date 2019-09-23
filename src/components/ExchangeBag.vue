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
        <span class="you">兑换红包</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->

    <!-- body -->
    <form class="item">
      <div class="item1">
        <input type="text" maxlength="10" placeholder="请输入兑换码" />
      </div>
      <div class="item2">
        <input type="text" maxlength="10" placeholder="验证码" />
        <div class="validate">
          <div>
            <img src="../assets/number.png" alt />
          </div>

          <div>
            <p>看不清</p>
            <p>换一张</p>
          </div>
        </div>
      </div>
    </form>
    <p class="exchange">兑换</p>

    <!-- body-end -->
  </div>
</template>

<script>
export default {
  name: "ExchangeBag",
  data() {
    return {
      validates: []
    };
  },
  created() {
    this.getValidate;
  },
  methods: {
    getValidate() {
      this.$axios
        .post(`https://elm.cangdu.org/v1/users/:user_id/hongbao/exchange`, {})
        .then(res => {
          console.log(res.data);
          this.validates = res.data;
        });
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
  margin-left: 0.6rem;
  margin-top: 0.7rem;
  margin-bottom: 0.7rem;
  height: 2rem;
  font-size: 0.7rem;
  color: #999;
  padding-left: 0.7rem;
  width: 15rem;
}
.item2 {
  display: flex;
}
.item2 input {
  margin-left: 0.6rem;
  height: 2rem;
  font-size: 0.7rem;
  color: #999;
  padding-left: 0.7rem;
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
.validate {
  background: #ffffff;
  font-size: 0.2rem;
  width: 6.4rem;
  height: 2rem;
  display: flex;
  margin-left: 0.3rem;
}
.validate img {
  width: 3.5rem;
  height: 1.5rem;
  margin-right: 0.2rem;
  margin-top: 0.3rem;
  margin-left: 0.2rem;
}
.validate div p {
  width: 3rem;
  text-align: center;
}
.validate div p:nth-child(1) {
  font-size: 0.55rem;
  color: #666;
  padding-top: 0.3rem;
}
.validate div p:nth-child(2) {
  color: #3b95e9;
  margin-top: 0.2rem;
}
</style>
