<template>
  <div class="Discount">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/BusinessVouchers">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">商家代金券说明</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <!-- body -->
    <div class="content">
      <h3>Q1：什么是商家代金券</h3>
      <ul>
        <li>商家代金券是指由商家自己发放代金券，只限在指定的商家使用，可根据条件抵扣相应金额</li>
      </ul>
      <h3>Q2：怎么获得商家代金券？</h3>
      <ul>
        <li>进入有进店领券或下单返券标识的商家即有机会获得代金券</li>
        <li>下单返券需要在指定商家完成满足返券金额要求的订单才会返还，代金券可在下次下单时使用</li>
      </ul>
      <h3>Q3：商家代金券使用条件？</h3>
      <ul>
        <li>商家代金券仅限在指定商家使用</li>
        <li>商家代金券仅限在限支付使用</li>
        <li>每个订单只能使用一张商家代金券，不可与其他代金券叠加使用</li>
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










