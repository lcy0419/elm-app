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
        <span class="you">准时达问题</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <h3>
        Q1:准时达规则：饿了么用户在饿了么APP带有准时达标签的商家下单，若商家送达时间超过承诺送达时间10分钟，我们将为您赔付一个无门槛红包。
        ### Q2：关于准时达的特殊情况：a.预订单暂不参加赔付；b.夜间部分时段下单暂不参加赔付；c.恶劣天气（雨、雪等）暂不参加赔付；d.每位用户每天最多赔付3个红包；
        ### Q3：常见问题 Q1:我怎么收到赔付红包？A1：当确认送达商品时已超过承诺送达时间10分钟，我们将向您的饿了么账户发放一个无门槛红包，同时会有短信通知到您的手机号码。
        ### 饿了么保留法律允许范围内对活动的解释权
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
