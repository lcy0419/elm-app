<template>
  <div class="scored-shop">
    <h3>请重新进入</h3>
    <p>请返回后重新进入积分商城~s</p>
    <span>
      <img src="../assets/retrylogin.png" alt />
    </span>
  </div>
</template>

<script>
export default {
  name: "ScoredShop"
};
</script>


<style scoped>
.scored-shop {
  margin-top: 8.75rem;
  margin-left: 1.3rem;
}
.scored-shop h3 {
  text-align: center;
  font-weight: bold;
  font-size: 26px;
  color: #0d7fd5;
  margin-bottom: 15px;
}
.scored-shop p {
  text-align: center;
  font-size: 14px;
  color: #666;
  margin-bottom: 19px;
}
.scored-shop span {
  width: 8rem;
  margin-left: 3.2rem;
}
.scored-shop img {
  width: 8rem;
  height: 8rem;
  vertical-align: middle;
}
</style>
