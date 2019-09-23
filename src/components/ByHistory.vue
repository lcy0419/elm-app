<template>
  <div class="buy-history">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/MenberCenter">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">购买记录</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->

    <!-- body -->
    <div class="content">
      <img src="../assets/下载.png" alt />
      <p>没有购买记录</p>
    </div>
    <!-- body-end -->
  </div>
</template>

<script>
export default {
  name: "ByHistory"
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
  left: 6rem;
}
.content {
  margin-top: 4rem;
  margin-left: 4.5rem;
}
.content img {
  width: 8rem;
  height: 5rem;
  margin-top: 5rem;
}
.content p {
  font-size: 0.6rem;
  color: #999;
  margin-top: 0.8rem;
  margin-left: 2.3rem;
}
</style>
