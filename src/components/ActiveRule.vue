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
        <span class="you">活动细则</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <h3>
        会员权益调整 尊敬的用户，随着会员服务体系优化，蜂鸟专送商家得到大规模普及，大大丰富了会员用户的用餐选择，从2016年9月1日开始，新购及续费的会员服务将由免配送费调整为每单最高减免4元配送费，之前购买的会员服务不受影响，感谢您的支持!
        敬请期待跟多会员特权。### Q1:特权介绍 * 减免配送：饿了么会员卡绑定账户，每日前3单在蜂鸟专送标识商家可减免配送费，每单最高可减4元。* 更多特权，敬请期待！### Q2：会员资费 * 月卡20元（一个月按31天计算）### Q3：购卡说明 * 在线购买：
        饿了么APP > 我的 > 饿了么会员卡。* 请认准饿了么官方认证渠道，任何从其他第三方途径获得的会员卡，饿了么不保证其可用性。
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
