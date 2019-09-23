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
        <span class="you">会员说明</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <h3>
        尊敬的用户，随着会员体系逐渐完善，自2016年10月10日起，饿了么会员权益将做如下优化：购卡后31天内，累计享有30单减免配送费服务（每日最多3单，每单最高减免4元）。>注：
        ：已购买的会员服务不受影响，当前会员服务失效前无法购买新卡。### Q1:特权介绍 * 身份标识：饿了么会员服务有效期内，享有专属皇冠标识。* 减免配送费：饿了么会员卡自绑定账户之日起31天内，
        在蜂鸟专送标识商家下单，享有30次减免配送费特权，每日最多减免3单，每单最多可减4元。* 更多特权，敬请期待！### Q2:资费介绍 * 饿了么会员卡：20元 ### Q3：使用说明 当用户满足以下任一条件，
        会员服务自动失效：1.自绑定之日起超过31天；2.在31天内累计使用减免配送费的蜂鸟订单数量达到30单；### Q4：购卡说明 * 在线购买：饿了么APP>我的>饿了么会员卡 ### Q5:温馨提示 * 用户在当前会员服务失效前，无法购买新卡。
        * 请认准饿了么官方渠道，任何从其他第三方途径获得的会员卡，饿了么不保证其可用性。
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
  font-size: 0.6rem;
  color: #333;
  font-weight: 400;
  padding: 1rem 1.3rem;
}
</style>
