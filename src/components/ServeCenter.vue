<template>
  <div class="serve-center">
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
        <span class="you">服务中心</span>
      </div>
      <!-- header-top-end -->

      <!-- header-body -->
      <div class="header-body">
        <div class="item1">
          <img src="../assets/客服.png" alt />
          <p>在线客服</p>
        </div>
        <div class="item2">
          <img src="../assets/客服电话.png" alt />
          <p>在线客服</p>
        </div>
      </div>
    </div>
    <!-- header-end -->
    <div class="content">
      <h4>热门问题</h4>
      <ul>
        <router-link to="/SuperMemberStatement">
          <li>
            <span>超级会员权益说明</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/AppearRule">
          <li>
            <span>签到规则</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/UserGradeStatement">
          <li>
            <span>用户等级说明</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/ScoreIssue">
          <li>
            <span>积分问题</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/Photograph">
          <li>
            <span>教我拍大片</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/PayStatement">
          <li>
            <span>支付问题</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/OtherIssue">
          <li>
            <span>其他问题</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/ArriveOnTime">
          <li>
            <span>准时达问题</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/VipStatement">
          <li>
            <span>会员说明</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/VipIssue">
          <li>
            <span>会员问题</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/Bag">
          <li>
            <span>红包问题</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/ActiveRule">
          <li>
            <span>活动细则</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/SupplementRule">
          <li>
            <span>补签规则</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/PreferentialStatement">
          <li>
            <span>优惠说明</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/ResponsibleStatement">
          <li>
            <span>负责声明</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/Voucher">
          <li>
            <span>代金券说明</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/Cooperate">
          <li>
            <span>商务合作</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/PayIssue">
          <li>
            <span>余额问题</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="SuperSeller">
          <li>
            <span>超赞商家</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/AnonymousBy">
          <li>
            <span>匿名购买</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
        <router-link to="/ActiveIssue">
          <li>
            <span>活动问题</span>
            <span>
              <img src="../assets/向右箭头 (4).png" alt />
            </span>
          </li>
        </router-link>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "BalanceStatement"
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
  padding-top: 3rem;
  display: flex;
  justify-content: space-around;
  background: #ffffff;
  /* border-right: 1px solid #f5f5f5; */
}
.item1 {
  border-right: 1px solid #f5f5f5;
  margin-left: 0.7rem;
}
.item1 img {
  width: 1rem;
  height: 1rem;
  margin-left: 0.7rem;
}
.item1 p {
  margin-top: 0.2rem;
  font-size: 0.6rem;
  color: #666;
  padding-bottom: 0.9rem;
}
.item2 {
  border-right: 1px solid #f5f5f5;
  margin-left: 0.7rem;
}
.item2 img {
  width: 1rem;
  height: 1rem;
  margin-left: 0.7rem;
}
.item2 p {
  margin-top: 0.2rem;
  font-size: 0.6rem;
  color: #666;
  padding-bottom: 0.5rem;
}
.content {
  background: #ffffff;
}
.content h4 {
  font-size: 0.75rem;
  color: #333;
  line-height: 3rem;
  border-bottom: 1px solid #f5f5f5;
  border-top: 1px solid #f5f5f5;
  padding-left: 0.7rem;
}
.content ul li {
  display: flex;
  padding: 0 0.7rem;
  line-height: 2rem;
  border-bottom: 1px solid #f5f5f5;
  justify-content: space-between;
  /* align-items: center; */
}
.content ul li span:nth-child(1) {
  font-size: 0.6rem;
  color: #666;
}
.content ul li span:nth-child(2) {
  width: 0.6rem;
  height: 0.6rem;
}
</style>
