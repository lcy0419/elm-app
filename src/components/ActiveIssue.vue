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
        <span class="you">活动问题</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <h3>
        Q1：使用余额的条件 为了保护账户安全，使用余额前必须先绑定手机号。### Q2：余额可以怎么用？余额可以在饿了么平台上提现 ，当余额大于等于待支付金额时可以在支持在线支付的商家中进行消费。提现功能将于2016年12月25日00：00全面开放。
        ### Q3：我要如何提现？为了保护账户和资金安全，您在提现时需要输入真实姓名和用该姓名开通的银行卡号、选择开户行、并验证已绑定饿了么账号的手机号。每日只能提现一次，每次限额50元。若提现金额超过50元，点击提现时系统会提示您已超额，请您修改提现金额。
        ### Q4:为什么会提现失败？可能原因有：您的姓名、开户行、银行卡号等信息不匹配；您当日的提现次数和金额超过限制；您的账户存在异常，被风控拦截。
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
