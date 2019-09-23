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
        <span class="you">我的优惠</span>
      </div>
      <!-- header-top-end -->

      <!-- header-body -->
      <div class="header-body">
        <router-link to="/RedBag">
          <span class="bag">红包</span>
        </router-link>
        <router-link to="/BusinessVouchers">
          <span class="business">商家代金券</span>
        </router-link>
      </div>
      <!-- header-body-end -->
    </div>
    <!-- header-end -->
    <!-- body -->
    <div class="body">
      <div class="item">
        <div class="item1-left"></div>
        <router-link to="/BusinessVouchersStatement">
          <div class="item1-right">
            <img src="../assets/问号.png" alt />
            商家代金券说明
          </div>
        </router-link>
      </div>
      <div class="item2">
        <p>
          <img src="../assets/man.png" alt />
        </p>
        <p>无法使用代金券</p>
        <p>非客户端或客户端版本过低</p>
        <router-link to="/DownLoad">
          <p class="client">下载或升级客户端</p>
        </router-link>
      </div>
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
.header-body {
  background: #ffffff;
  padding-top: 2.5rem;

  padding-bottom: 0.5rem;
  text-align: center;
  font-size: 0.65rem;
  display: flex;
  justify-content: space-around;
}
.business {
  color: #3190e8;
  border-bottom: 2px solid #3190e8;
  padding-bottom: 0.3rem;
}
.item1 {
  display: flex;
  justify-content: space-between;
}
.item1-right {
  font-size: 0.5rem;
  line-height: 2rem;
  color: #3190e8;
  margin-left: 11rem;
}
.item2 {
  text-align: center;
  margin-top: 4rem;
}
.item2 img {
  width: 6rem;
  height: 3.4rem;
}
.item2 p:nth-child(2) {
  font-size: 0.7rem;
  color: #666;
  margin-top: 0.4rem;
}
.item2 p:nth-child(3) {
  font-size: 0.5rem;
  color: #999;
  margin-top: 0.3rem;
  margin-bottom: 0.3rem;
}
.client {
  background-color: #56d176;
  font-size: 0.65rem;
  color: #fff;
  padding: 0.3rem;
  border-radius: 0.15rem;
  width: 10rem;
  margin-left: 3rem;
}
</style>










