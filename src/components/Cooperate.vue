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
        <span class="you">商务合作</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <h3>
        Q1：我是新用户，为什么不能享受新用户下单立减优惠/新用户首单红包？* 新用户是指您的下单设备、手机号、饿了么账号、支付账号、都是第一次在饿了么平台使用。
        以上任意条件不满足，都不能享受新用户优惠。* 如果监测到您不满足以上的信用条件，您的订单将会被系统拦截或者无偿取消。* 新用户立减优惠、新用户红包、满减特价菜活动不能同时使用。
        在您首次下单过程中，我们会优先为您选择优惠最大（优惠金额最高）的。### Q2：首单被取消，再次下单还能享受新用户立减优惠/新用户红包吗？* 您主动取消或商家、骑手取消的订单，饿了么会返还您的新用户资格，
        这是您仍然可以享受新用户的优惠。*您被取消的首单因为使用的支付账户曾下过单，必须更换新的支付账户才可以享受新用户优惠。* 但您取消的原因是账户异常等原因，则不能享受新用户优惠。
        ### Q3：我第一次在 "A" 商家下单，"A" 商家有参加新用户活动，我为什么享受不到新用户的立减优惠？* 活动中的新用户指的是饿了么网站的新用户，而不是指 "A" 商家的新客户。如果您不符合饿了么网站新用户的定义则无法享受与新用户相关的活动优惠。
        ### Q4：一个红包能拆开多次使用吗？* 不能，一个红包只能一次性使用，不能分开使用。### Q5：下单的时候使用了红包，但是后来订单取消了，红包还会返还吗？* 会的，订单无效后红包会自动返还到您的账户里。### Q6：红包兑换码怎样兑换成红包，怎样查看红包？
        * 在个人中心 > 我的钱包 > 兑换红包，输入兑换码进行兑换。### Q7：在线支付订单取消后，钱怎么返还？* 使用饿了么账户余额支付，订单无效后，所有款项将退到您的饿了么账户；使用第三方支付订单无效后，支付款项将于两个工作日内返还到您的第三方支付账户，红包退还到饿了么账户。
        ### Q8：每天限制优惠3单，前面下了一个在线支付的单子，由于未付款，订单自动取消了，这单会计算我的参与活动次数吗？* 不会。未付款的订单不会计入您使用优惠的次数。### Q9：每天红包使用次数有限制吗？* 同一个手机号每天最多能使用两个红包优惠（不含预定早餐和预定午餐），使用红包的订单
        出现退单情况不计入限制。
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
  margin: 0 0.6rem;
  margin-top: 2rem;
}
h3 {
  display: block;
  font-size: 0.7rem;
  color: #333;
  font-weight: 400;
  padding: 0 0.35rem;
}
</style>
