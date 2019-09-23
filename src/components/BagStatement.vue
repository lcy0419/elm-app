<template>
  <div class="Discount">
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
        <span class="you">红包说明</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <!-- body -->
    <div class="content">
      <h3>Q1：怎么获得红包</h3>
      <ul>
        <li>通过邀请好友获得</li>
        <li>在下单返红包的商家下单获得</li>
        <li>抢微信朋友分享的红包获得</li>
      </ul>
      <h3>Q2：红包可以做什么？</h3>
      <ul>
        <li>可以抵扣在线支付时的实际支付金额</li>
      </ul>
      <h3>Q3：红包的门槛金额按照什么什么金额计算？</h3>
      <ul>
        <li>红包的门槛金额按照（选购菜品折后价 + 餐盒费）的金额作为计算门槛，即购物车显示的余额（7.3以上版本）。假设红包满30可用，只要选购的菜品现价（折后价）+ 餐盒费超过30，就可以使用红包。</li>
      </ul>
      <h3>Q4：一个红包能拆开多次使用吗？</h3>
      <ul>
        <li>不能，一个红包只能一次性使用，不能分开使用</li>
      </ul>
      <h3>Q5：下单的时候使用了红包，但是后来订单取消了，红包还会返还吗？</h3>
      <ul>
        <li>会的，订单无效后红包会自动返还到您的账户里。</li>
      </ul>
      <h3>Q6：红包的兑换码怎样兑换成红包，怎样查看红包？</h3>
      <ul>
        <li>在个人中心 > 我的红包 > 兑换红包，输入兑换码进行兑换</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Discount"
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
  left: 5.5rem;
}
.content {
  padding-top: 2rem;
  padding-left: 0.6rem;
  padding-right: 0.3rem;
}
.content h3 {
  line-height: 2rem;
  color: #333;
  font-size: 0.75rem;
  font-weight: 500;
}
.content ul li {
  font-size: 0.6rem;
  color: #666;
  line-height: 1rem;
}
</style>










