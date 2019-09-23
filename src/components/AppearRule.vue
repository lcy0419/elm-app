<template>
  <div class="down-load">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/ServeCenter">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">签到规则</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <h3>
        <p>如何签到领红包 用户需要支付 1 元参与活动 （后续签到不收费）</p>
        <p>活动期间每日签到，9天后即可领取 10 元无门槛红包</p>
        <p>如期间忘记签到，可领红包金额会减少，详细如下</p>
        <p>
          -
          <strong>完成9天签到：</strong>10元（2个5元红包）-
          <strong>漏签1天：</strong>8元（2个4元红包）-
          <strong>漏签2天：</strong>6元（2个3元红包）-
          <strong>漏签3天：</strong>4元（2个2元红包）-
          <strong>漏签4天及以上：</strong>1个2元红包
        </p>
        <p>
          ###漏签后如何补签 如忘记签到，可通过下单补签，漏签当日至红包领取日前一天每一笔有效订单可补签1天（
          仅限在线支付订单），例：如您在活动第三天忘记签到，只要你在第三天至第九天内完成1笔有效订单，即可完成补签。
          ###每日签到拿福利：-签到期间，每日 10：30 可抢 5 元红包，每日限领一个。红包数量有限，抢完为止，要记得来早哦~
        </p>
      </h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "DownLoad"
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
  left: 5.3rem;
}
.content {
  margin-top: 2rem;
  margin-left: 0.8rem;
  margin-right: 0.8rem;
}
h3 p {
  display: block;
  font-size: 0.8rem;
  color: #333;
}
strong {
  font-weight: bold;
}
</style>
