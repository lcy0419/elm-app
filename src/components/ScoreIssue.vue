<template>
  <div class="balance-statement">
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
        <span class="you">积分问题</span>
      </div>
      <!-- header-top-end -->

      <!-- body -->
      <div class="content">
        <div class="item1">
          <h3 class="title">Q1:怎么获得积分</h3>
          <p class="content-body">在线支付的订单将获得订单积分奖励：</p>
          <p class="content-body">积分将在用户完成评价后获得</p>
          <p class="content-body">可获得积分=订单金额*10（即1元=10点积分）。</p>
          <p class="content-body">订单金额指实际付款金额，不包含活动优惠金额。</p>
          <p class="content-body">每位用户每天最多可获得2000积分，体验商家的订单和评价不会增加积分。</p>
        </div>
        <div class="item2">
          <h3 class="title">Q2:积分用来做什么?</h3>
          <p class="content-body">可以在积分商城兑换各种礼品</p>
        </div>
        <div class="item3">
          <h3 class="title">Q3:礼品兑换很多天了还没有收到，该怎么办?</h3>
          <p class="content-body">礼品从兑换日起，3个工作日（周末不算）内处理发货，发货后，通常会在3个工作日左右送达</p>
        </div>
        <div class="item4">
          <h3 class="title">Q4:礼品兑换中的手机充值卡兑换，怎么样进行充值，充值之前会和我电话确认吗?</h3>
          <p class="content-body">不会，手机充值卡兑换，是直接充值到您填写的手机号上，充值之前不会和您电话确认，所以您在填写电话的时候，请确认电话是否正确。</p>
        </div>
      </div>
      <!-- body-end -->
    </div>
    <!-- header-end -->
  </div>
</template>

<script>
export default {
  name: "BalanceStatement"
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
.content {
  margin-top: 2.3rem;
  margin-left: 0.6rem;
  margin-right: 0.6rem;
}
.title {
  line-height: 2rem;
  color: #333;
  font-weight: 400;
  font-size: 0.75rem;
}
.content-body {
  font-size: 0.6rem;
  color: #666;
  line-height: 1rem;
}
</style>
