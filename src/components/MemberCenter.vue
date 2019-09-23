<template>
  <div class="member-center">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/My">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">会员中心</span>
      </div>
      <!-- header-top-end -->

      <!-- header-body -->
      <div class="header-body">
        <p>
          为账户
          <span>1169337554</span>购买会员
        </p>
      </div>
      <!-- header-body-end -->
    </div>
    <!-- header-end -->

    <!-- body -->
    <div class="item1">
      <router-link to="DiscountStatement">
        <div class="item1-header">
          <span>会员特权</span>
          <span>
            会员说明
            <img src="../assets/right.png" alt />
          </span>
        </div>
      </router-link>

      <div class="item1-body">
        <div>
          <img src="../assets/save.jpg" alt />
        </div>
        <div>
          <h4>减免配送费</h4>
          <p>每月减免30单。每日可减免3单，每单最高减4元</p>
          <p>蜂鸟专送专享</p>
        </div>
      </div>
      <div class="item1-body">
        <div>
          <img src="../assets/bag.jpg" alt />
        </div>
        <div>
          <h4>减免配送费</h4>
          <p>每月减免30单。每日可减免3单，每单最高减4元</p>
          <p>蜂鸟专送专享</p>
        </div>
      </div>
    </div>
    <div class="item2">
      <p>开通会员</p>
      <div class="shop">
        <div>
          <span>1个月</span>
          <span>￥20</span>
        </div>
        <div>
          <router-link to="/PayFor">
            <span>购买</span>
          </router-link>
        </div>
      </div>
    </div>
    <router-link to="/ExchangeMember">
      <div class="item3">
        <span>兑换会员</span>
        <span>
          使用卡号卡密
          <img src="../assets/right.png" alt />
        </span>
      </div>
    </router-link>

    <router-link to="/ByHistory">
      <div class="item3">
        <span>购买记录</span>
        <span class="tip">
          开发票
          <img src="../assets/right.png" alt />
        </span>
      </div>
    </router-link>

    <!-- body-end -->
  </div>
</template>

<script>
export default {
  name: "MemberCenter"
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
.header-body {
  position: relative;
  top: 2rem;
}
.header-body p {
  font-size: 0.6rem;
  color: #666;
  line-height: 2rem;
  padding-left: 0.7rem;
}
.header-body span {
  font-weight: 700;
  padding-right: 0.3125rem;
}
.item1 {
  margin-top: 2rem;
  background: #ffffff;
}
.item1-header {
  display: flex;
  justify-content: space-around;
  border-bottom: 1px solid #f5f5f5;
}
.item1-header span {
  line-height: 2rem;
}
.item1-header span:nth-child(1) {
  font-size: 0.7rem;
  color: #333;
  margin-left: -3.5rem;
}
.item1-header span:nth-child(2) {
  font-size: 0.6rem;
  color: #999;
  margin-right: -3.5rem;
}
.item1-body {
  display: flex;
  justify-content: space-around;
  padding: 1rem 0;
  border-bottom: 1px solid #f5f5f5;
}
.item1-body div:nth-child(1) img {
  width: 1.6rem;
  height: 1.8rem;
  margin-left: -1.5rem;
}
.item1-body div:nth-child(2) {
  margin-left: -3.5rem;
}
.item1-body div:nth-child(2) h4 {
  font-size: 0.7rem;
  color: #333;
  font-weight: 400;
}
.item1-body div:nth-child(2) p {
  font-size: 0.5rem;
  color: #999;
}
.item2 {
  margin-top: 0.6rem;
  background: #ffffff;
}
.item2 p {
  font-size: 0.7rem;
  color: #333;
  line-height: 2rem;
  margin-left: 0.7rem;
  border-bottom: 1px solid #f5f5f5;
}
.shop {
  display: flex;
  justify-content: space-around;
  line-height: 2rem;
}
.shop div:nth-child(1) {
  margin-left: -3.5rem;
}
.shop div:nth-child(2) {
  margin-right: -2.5rem;
  border: 0.025rem solid #f60;
  border-radius: 0.2rem;
  line-height: 1.2rem;
  height: 1.2rem;
  width: 2.6rem;
  text-align: center;
  font-size: 0.6rem;
  color: #f60;
  margin-top: 0.5rem;
}
.shop div:nth-child(2) span {
  color: #f60;
}
.shop div:nth-child(1) span {
  margin-left: 0.3rem;
}
.shop div:nth-child(1) span:nth-child(1) {
  font-size: 0.7rem;
  color: #333;
}
.shop div:nth-child(1) span:nth-child(2) {
  font-size: 0.7rem;
  font-weight: 700;
  color: #f60;
}
.item3 {
  padding: 0 0.7rem;
  margin-bottom: 0.5rem;
  background: #ffffff;
  margin: 0.6rem 0;
}
.item3 span {
  line-height: 2rem;
}
.item3 span:nth-child(1) {
  font-size: 0.7rem;
  color: #333;
  margin-right: 7rem;
}
.item3 span:nth-child(2) {
  font-size: 0.6rem;
  color: #999;
  margin-right: 0.2rem;
}
.item3 .tip {
  margin-left: 1.5rem;
}
</style>
