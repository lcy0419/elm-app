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
        <span class="you">负责声明</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <h3>
        新用户是根据设备、饿了么账号、下单手机号进行判断，如果您下单时以上信息均为首次使用则符合饿了么定义的新用户 * 仅限新用户使用移动端app提交订单并选择在线支付时享受
        （饿配送订单选择餐到付款也可享受）* 在本设备上曾经有过购买记录的行为的手机不能参加本活动 * 新用户首单立减金额各领域不同 * 活动仅支持手机客户端最新版本
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
