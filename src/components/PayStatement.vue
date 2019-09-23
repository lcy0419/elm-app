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
        <span class="you">支付问题</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <h3>
        Q1:使用余额支付不了？先确认下您的饿了么账户是否有绑定手机号，使用余额支付必须先绑定手机号。### Q2：在线支付订单取消后，钱怎么返还？使用饿了么账户余额支付（
        包括：余额、余额 + 红包），订单无效后，所以款项（包括红包）将退到您的饿了么账户；使用第三方支付（包括第三方支付
        、第三方支付 + 红包），订单无效后，支付款项将于2个工作日内返还到您的第三方支付账户，红包退还到饿了么账户。### Q3：在线支付过程中，订单显示未支付成功，款项却被扣了，该怎么办？
        该问题属于第三方（银行/支付宝/微信等）数据传输延迟问题。您可以再等待一下，如果超过半小时，订单还是未支付状态，第三方会把款项返还到您的支付账户。具体到账时间依银行而定，一般会在两个工作日内，
        ### Q4：每天限制优惠3单，前面下了一个在线支付的单子，由于未付款，订单自动取消了，这单子会计算我的参与活动次数吗？
        不会，您可以在订单列表页或者订单详情页查看，当订单状态变为订单已取消时，系统会自动~将您之前享受的优惠返还到您的账户中，下一次下单依然可以使用。自己取消订单、超时未付款自动取消订单、商家取消订单，
        这些情况都会返还优惠次数。### Q5：饿了么账户里的款项怎么提现？在操作中心 > 我的余额 > 提现处进行提现操作。
        操作日起两个工作日内，款项会返还至您最近消费过的账户中。### Q6：支付宝免密支付功能如何使用？首次进入支付收银台并使用支付宝支付时，系统会默认进入免密支付的签约页面，您可以根据自身支付喜好选择是否签约免密支付功能。
        如您不签约该功能，之后会默认使用正常支付宝支付流程。此外，您还可以通过 "个人中心" - "小额免密支付" 中的免密支付开关，随时进行 "签约"、"解约" 支付宝免密支付操作。
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
  font-size: 0.75rem;
  color: #333;
  font-weight: 400;
  padding: 0 0.35rem;
}
</style>
