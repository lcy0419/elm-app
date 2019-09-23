<template>
  <div class="down-load">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/AddAddress">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">搜索地址</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <div>
        <input type="text" placeholder="请输入小区/写字楼/学校等" />
        <button>确认</button>
      </div>
    </div>
    <div class="shop">为了满足商家的送餐要求，建议您从列表中选择地址</div>
    <div class="line">
      <ul>
        <li>
          <p></p>
          <p></p>
        </li>
      </ul>
    </div>
    <div class="footer">
      <p>找不到地址?</p>
      <p>请尝试输入小区、写字楼或学校名</p>
      <p>详细地址（如门牌号）可稍后输入哦。</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "DownLoad",
  data() {
    return {};
  },
  methods: {}
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
  margin-top: 2.5rem;
  background: #fff;
}
.content div:nth-child(1) {
  display: flex;
  justify-content: space-between;
  background: #fff;
  padding: 0.5rem;
}
.content div:nth-child(1) input {
  display: block;
  width: 11.8rem;
  padding: 0.4rem;
  background: #f2f2f2;
  border: 1px solid #ddd;
  border-radius: 5px;
  font-size: 0.6rem;
}
.content div:nth-child(1) button {
  display: block;
  width: 3rem;
  background: #3199e8;
  font-size: 0.7rem;
  color: #fff;
  border-radius: 5px;
}
.shop {
  background: #fff6e4;
  font-size: 0.62rem;
  color: #ff883f;
  text-align: center;
  padding: 0.2rem 0;
}
.line ul li {
  border-bottom: 1px solid #ccc;
  padding: 0.4rem;
}
.line ul li p:nth-child(1) {
  margin-bottom: 0.2rem;
}
.line ul li p:nth-child(2) {
  font-size: 0.65rem;
  color: #969696;
}
.footer {
  margin-top: 4rem;
}
.footer p {
  width: 100%;
  text-align: center;
  font-size: 0.7rem;
  color: #969696;
  margin-bottom: 0.4rem;
}
</style>
