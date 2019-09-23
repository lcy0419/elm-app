<template>
  <div class="down-load">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/AccountInformation">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">重置密码</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <div>
        <input type="text" placeholder="账号" maxlength="11" />
      </div>
      <div>
        <input type="text" placeholder="旧密码" />
      </div>
      <div>
        <input type="text" placeholder="请输入新密码" />
      </div>
      <div>
        <input type="text" placeholder="请确认密码" />
      </div>
      <div class="verfily">
        <input type="text" placeholder="验证码" />
        <div class="ima">
          <img src="../assets/ima.png" alt />
          <div>
            <p>看不清</p>
            <p>换一张</p>
          </div>
        </div>
      </div>
    </div>

    <div class="footer" @click="change">确认修改</div>

    <!-- 弹窗 -->
    <div class="medium" v-show="this.confirm">
      <div class="medium-header">
        <img src="../assets/感叹号.png" alt />
        <p>请输入正确的账号</p>
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
      confirm: false
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
.content div {
  padding: 0.3rem 0.8rem;
  border-bottom: 1px solid #f1f1f1;
}
.content input {
  font-size: 0.7rem;
  color: #666;
}
.verfily {
  display: flex;
  padding: 0.3rem 0.8rem;
  border-bottom: 1px solid #f1f1f1;
}
.verfily input {
  font-size: 0.7rem;
  color: #666;
  height: 1.5rem;
}
.footer {
  margin: 1rem 0.5rem;
  font-size: 0.7rem;
  color: #fff;
  background-color: #4cd964;
  padding: 0.5rem 0;
  border: 1px;
  border-radius: 0.15rem;
  text-align: center;
}
.ima {
  margin-left: -2rem;
  position: absolute;
  right: -1rem;
  top: 10rem;
  display: flex;
}
.ima img {
  width: 3.5rem;
  height: 1.5rem;
  margin-left: 0rem;
  margin-top: 0.4rem;
}
.ima div {
}
.ima div {
  /* margin-right: 1rem; */
}
.ima div p:nth-child(1) {
  font-size: 0.55rem;
  color: #666;
}
.ima div p:nth-child(2) {
  font-size: 0.55rem;
  color: #3b95e9;
  margin-top: 0.2rem;
}
.medium {
  display: flex;
  flex-direction: column;
  position: absolute;
  animation: 0.4s;
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
