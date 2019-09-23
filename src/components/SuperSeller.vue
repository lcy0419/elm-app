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
        <span class="you">超赞商家</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <h3>
        Q1：什么是商家代金券？商家代金券是指由商家自己发放代金券，只限在指定的商家使用，可根据条件抵扣相应金额。### Q2：怎么获得商家代金券？
        * 进入有进店领券或下单返券标识的商家即有机会获得代金券。* 下单返券需要在指定商家完成满足返券金额要求的订单后才会返还，代金券可在下次下单时使用。
        ### Q3：商家代金券使用条件 * 商家代金券仅限在指定商家使用 * 商家代金券仅限在线支付时使用 * 每个订单只能使用一张商家代金券，不可与其他代金券叠加使用
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
