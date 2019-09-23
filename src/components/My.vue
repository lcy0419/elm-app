<template>
  <div class="my">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <a href>
            <img src="../assets/左箭头.png" alt="左箭头" />
          </a>
        </span>
        <span class="you">我的</span>
      </div>
      <!-- header-top-end -->

      <!-- header-body -->
      <router-link to="/AccountInformation">
        <div class="header-body clear">
          <div class="people left">
            <img src="../assets/people.png" alt />
          </div>
          <div class="left">
            <p class="login clear">
              <span class="left">登录/</span>
              <span class="left">注册</span>
            </p>
            <p class="phone">
              <span>
                <img src="../assets/phone.png" alt />
              </span>
              <span>暂无绑定手机号</span>
            </p>
          </div>

          <div class="arrow right">
            <img src="../assets/向右箭头.png" alt />
          </div>
        </div>
      </router-link>
      <!-- header-body-end -->
    </div>
    <!-- header-end -->

    <!-- body -->
    <div class="body clear">
      <!-- item1 -->
      <div class="item1">
        <ul>
          <li>
            <router-link exact to="/Money">
              <span>
                <b>0.00</b>
                <span class="title">元</span>
              </span>
              <p>我的余额</p>
            </router-link>
          </li>
          <li>
            <router-link exact to="/Discount">
              <span>
                <b>3</b>
                <span class="title">个</span>
              </span>
              <p>我的优惠</p>
            </router-link>
          </li>
          <li>
            <router-link exact to="/Scored">
              <span>
                <b>0</b>
                <span class="title">分</span>
              </span>
              <p>我的积分</p>
            </router-link>
          </li>
        </ul>
      </div>
      <!-- item1-end -->

      <!-- item2 -->
      <div class="item2 clear">
        <ul>
          <router-link to="/List">
            <li>
              <span class="ph">
                <img src="../assets/订单.png" alt />
              </span>
              <span>我的订单</span>
              <a href="#" class="right">
                <img src="../assets/right.png" alt />
              </a>
            </li>
          </router-link>

          <router-link to="/ScoredShop">
            <li>
              <span class="ph">
                <img src="../assets/shop.png" alt />
              </span>
              <span>积分商城</span>
              <a href="#" class="right">
                <img src="../assets/right.png" alt />
              </a>
            </li>
          </router-link>

          <router-link to="/MenberCenter">
            <li>
              <span class="ph">
                <img src="../assets/win.png" alt />
              </span>
              <span>饿了么会员卡</span>
              <a href="#" class="right">
                <img src="../assets/right.png" alt />
              </a>
            </li>
          </router-link>
        </ul>
      </div>
      <!-- item2-end -->

      <!-- item3 -->
      <div class="item3">
        <ul>
          <router-link to="/ServeCenter">
            <li>
              <span class="ph">
                <img src="../assets/左边小正方形.png" alt />
              </span>
              <span>服务中心</span>
              <a href="#" class="right">
                <img src="../assets/right.png" alt />
              </a>
            </li>
          </router-link>

          <router-link to="/DownLoad">
            <li>
              <span class="ph">
                <img src="../assets/饿了么.png" alt />
              </span>
              <span>下载饿了么APP</span>
              <a href="#" class="right">
                <img src="../assets/right.png" alt />
              </a>
            </li>
          </router-link>
        </ul>
      </div>
      <!-- item3-end -->

      <!-- footer -->
      <footer class="clear">
        <ul>
          <li class="left">
            <span>
              <img src="../assets/外卖.png" alt />
            </span>
            <p>外卖</p>
          </li>
          <li class="left">
            <span>
              <img src="../assets/指南针.png" alt />
            </span>
            <p>搜索</p>
          </li>
          <li class="left">
            <span>
              <img src="../assets/sh.png" alt />
            </span>
            <p>订单</p>
          </li>
          <li class="left">
            <span>
              <img src="../assets/人.png" alt />
            </span>
            <p>我的</p>
          </li>
        </ul>
      </footer>
    </div>
    <!-- body-end -->
  </div>
</template>

<script>
export default {
  name: "My"
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
  left: 6.5rem;
}
.header-body {
  border-top: 1px solid #f1f1f11c;
  background-color: #3190e8;
  top: 1.9rem;
  position: relative;
  width: 100%;
  align-items: center;
  padding: 0.666667rem 0.6rem;
  z-index: 100;
  overflow: hidden;
  padding-left: 0.7rem;
  padding-top: 0.7rem;
}
.header-body span {
  color: #fff;
}
.people {
  width: 2.5rem;
  height: 2.5rem;
}
.people img {
  width: 100%;
  height: 100%;
}
.login span {
  font-weight: 700;
  font-size: 0.8rem;
}
.login {
  position: absolute;
  margin-top: 0.3rem;
  margin-left: 0.5rem;
}
.phone {
  position: relative;
  top: 1.7rem;
  font-size: 0.57333rem;
  left: 0.3rem;
}
.phone span:nth-child(2) {
  position: relative;
  top: -0.1rem;
  margin-left: 0.2rem;
}
.arrow {
  position: relative;
  right: 1.5rem;
  top: 0.5rem;
}
.left {
  float: left;
}
.right {
  float: right;
}
.clear {
  overflow: hidden;
}
/* body */
.body {
  position: relative;
  top: 3rem;
}
.item1 ul {
  display: flex;
  justify-content: space-around;
}
.item1 ul li {
  text-align: center;
}
.item1 ul li p {
  font-size: 0.57333rem;
  color: #666;
  font-weight: 400;
}
.item1 ul li b {
  font-size: 1.2rem;
  font-weight: 700;
  line-height: 1rem;
  font-family: Helvetica Neue, Tahoma;
}
.title {
  font-size: 0.57333rem;
  color: #666;
  font-weight: 400;
}
.item1 ul li:nth-child(1) b {
  color: #f90;
}
.item1 ul li:nth-child(2) b {
  color: #ff5f3e;
}
.item1 ul li:nth-child(3) b {
  color: #6ac20b;
}
.item2 ul {
  margin-top: 1rem;
}
.item2 ul li {
  height: 2.5rem;
  line-height: 2.68rem;
  border-bottom: 1px solid #f1f1f1;
}
.ph {
  margin-left: 0.7rem;
  margin-right: 0.5rem;
}
.item2 ul li span {
  font-size: 0.7rem;
}
.item2 ul li a {
  position: absolute;
  right: 1rem;
}
.item3 ul {
  margin-top: 0rem;
}
.item3 ul li {
  height: 2.5rem;
  line-height: 2.68rem;
  border-bottom: 1px solid #f1f1f1;
}
.item3 ul li span {
  font-size: 0.7rem;
}
.item3 ul li a {
  position: absolute;
  right: 1rem;
}

footer ul {
  margin-top: 4.6rem;
  display: flex;
  justify-content: space-around;
}
footer ul li {
  text-align: center;
  font-size: 0.45rem;
  color: #666;
  font-weight: 400;
}
</style>
