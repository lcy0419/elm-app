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
        <span class="you">用户等级说明</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <p>
        用户等级是你在饿了么的身份表现，为了感谢您长期以来对饿了么的信赖和支持，我们会根据您的等级回馈相应的福利和特权，功能还在内测中，暂定规则如下：
        ###用户等级的划分：用户等级按月度计算，每个自然月的最后一天会统计你当月的累计消费金额（限在线支付金额，不包含活动优惠及红包及代金券抵扣），决定你次月的等级
        具体要求如下。*LV0 月累计消费100元以下；*LV1月累计消费大于等于100，小于200元，*LV2月累计消费大于等于200，小于500元 *LV3月累计消费大于等于500
        ###升级及降级规则：每笔订单完成后，系统会自动计算你当月有效的消费金额（限在线支付金额，不包含活动优惠及红包及代金券抵扣），当月累计消费一旦达到下一等级要求，我们会立刻为您升级，
        您及时就可享受新等级的相关权益。
      </p>
      <p>如您本月累计消费金额未达到当前等级要求，次月您将被降到与本月消费相匹配的等级。*内测期间饿了么会调整等级权益及规则，饿了么保留对等级体系的所有解释权。</p>
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
  left: 4.3rem;
}
.content {
  margin: 0 0.6rem;
  margin-top: 2rem;
}
.content p {
  display: block;
  columns: #333;
  font-size: 0.7rem;
  font-weight: 400;
}
</style>
