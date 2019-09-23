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
        <span class="you">超级会员权益说明</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <h2>
        什么时超级会员 超级会员是饿了么为了更好的服务用户，推出的一项增值会员服务，包含众多会员专属权益，全面提升核心用户购物体验
        ，加入会员后您将获得以下会员特权：###专享红包 *当月购买当月生效，可立即获得四张面额5元的饿了么红包，
        总计20元；*发放的四个红包皆无使用金额要求，全品类通用（早餐及帮买帮送等特殊订单除外）；*其中有两个红包限蜂鸟专送使用
        ，其余红包无配送要求；*发放的红包使用日期有区别，相隔14天，也就是有两个红包发放日当日即可使用，有两个需14
        天后才能使用。###下单奖励 * 每完成5笔在线支付订单，更可领取5元红包，下单越多可领取的红包越多！ *奖励的红包
        无使用金额要求，全品类通用（早餐及帮买帮送订单除外）。###专属活动 *针对会员不定期会推出专属活动，可享受会员
        折扣商品，可获得专属红包及商家代金券活动。###积分特权 *积分商城的会员专区将为超级会员不定期推出专属礼品
        ，优惠多多，豪礼多多！##常见问题 ###常见会员是否有配送费优惠？ *超级会员暂无配送费优惠政策，配送费按
        商家定价收取。###为何没收到会员专享红包？*专享红包按月发放，如用户购买多月会员，则每月会员生效日可获得
        对应四个专享红包。###如何获得下单奖励红包？*会员有效期内，用户每完成5笔在线支付订单，用户可去会员主页领取5元红包。如
        会员已过期，则无法领取。###超级会员如何退订？*会员到期后，如用户不再续费则自动退订，会员有效期内无法退订会员，已缴纳的会费不能返还
        。###红包有无使用限制？*专享红包及下单奖励红包无金额门槛要求，但每笔订单需最少支付0，01元；*没个红包只能使用
        一次，不能叠加或拆分使用；*红包需在有效期内使用，过期红包即刻失效，请注意红包有效期；*每月专享红包中，
        有两个红包有配送限制，订单需为蜂鸟专送方可使用，其余红包无配送限制。
      </h2>
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
  left: 4.3rem;
}
.content {
  margin-top: 2rem;
}
h2 {
  display: block;
  font-size: 1em;
  margin-block-start: 0.83em;
  margin-block-end: 0.83em;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  color: #333;
  margin: 0 1rem;
}
</style>
