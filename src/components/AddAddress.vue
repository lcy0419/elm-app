<template>
  <div class="down-load">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/Address">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">新增地址</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <input type="text" placeholder="请输入你的姓名" />
      <router-link to="/SelectAddress">
        <input type="text" placeholder="小区/写字楼/学校等" />
      </router-link>

      <input type="text" placeholder="请填写详细送餐地址" />
      <input type="text" placeholder="请填写能够联系到您的手机号" />
      <input type="text" placeholder="备用电话（选填）" />
    </div>
    <div class="footer" @click="change">
      <button>新增地址</button>
    </div>

    <!-- 弹窗 -->
    <div class="medium" v-show="this.confirm">
      <div class="medium-header">
        <img src="../assets/感叹号.png" alt />
        <p>地址信息错误</p>
      </div>
      <div class="medium-footer">
        <p @click="change1">确认</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "DownLoad",
  data() {
    return {
      ended: false,
      confirm: false,
      phone: false
    };
  },
  methods: {
    change() {
      this.confirm = true;
    },
    change1() {
      this.confirm = false;
    }
  }
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
.content input {
  display: block;
  width: 15rem;
  font-size: 0.6rem;
  margin: 0 auto;
  padding: 0.3rem;
  background: #f2f2f2;
  border: 1px solid #ddd;
  border-radius: 3px;
  margin-top: 0.5rem;
}
.footer button {
  width: 15rem;
  font-size: 0.6rem;
  color: #fff;
  line-height: 1.6rem;
  background: #4cd964;
  font-weight: 700;
  opacity: 0.6;
  margin-top: 1rem;
  margin-left: 0.7rem;
}
.medium {
  display: flex;
  flex-direction: column;
  position: absolute;
  top: 50%;
  left: 50%;
  margin-top: -6rem;
  margin-left: -6rem;
  width: 12rem;
  animation: tipMove 0.4s;
  background-color: #fff;
  padding-top: 0.6rem;
  border: 1px;
  border-radius: 0.25rem;
}
.medium-header img {
  position: relative;
  width: 3rem;
  height: 3rem;
  border-radius: 50%;
  top: 0.5rem;
  left: 4.5rem;
}
.medium-header p {
  font-size: 0.7rem;
  color: #333;
  line-height: 0.9rem;
  text-align: center;
  margin-top: 0.8rem;
  padding: 0 0.4rem;
}
.medium-footer {
  font-size: 0.8rem;

  font-weight: 700;
  margin-top: 0.8rem;
  background-color: #4cd964;
  width: 100%;
  text-align: center;
  line-height: 1.8rem;
  border: 1px;
  border-bottom-left-radius: 0.25rem;
  border-bottom-right-radius: 0.25rem;
}
.medium-footer p {
  color: #fff;
}
</style>
