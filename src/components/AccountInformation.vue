<template>
  <div class="Account-information">
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
        <span class="you">账户信息</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <div @click="change2">
        <input type="file" class="upload" />
        <h2>头像</h2>
        <div class="upload-img">
          <img src="../assets/upload.jpg" alt />
          <span>
            <img src="../assets/right.png" alt />
          </span>
        </div>
      </div>
      <router-link to="/ChangeUserName">
        <div>
          <h2>用户名</h2>
          <div class="user">
            <p>{{username}}</p>
            <span>
              <img src="../assets/right.png" alt />
            </span>
          </div>
        </div>
      </router-link>
      <router-link to="/Address">
        <div>
          <h2>收货地址</h2>
          <div class="user">
            <span>
              <img src="../assets/right.png" alt />
            </span>
          </div>
        </div>
      </router-link>

      <div>账户绑定</div>
      <div class="phone" @click="change3">
        <div>
          <img src="../assets/mobilphone.png" alt />
          <h2>手机</h2>
        </div>
        <div class="user">
          <span>
            <img src="../assets/right.png" alt />
          </span>
        </div>
      </div>
      <div>安全设置</div>
      <router-link to="/ResetPassword">
        <div>
          <h2>登录密码</h2>
          <div class="user">
            <p>修改</p>
            <span>
              <img src="../assets/right.png" alt />
            </span>
          </div>
        </div>
      </router-link>

      <div @click="change">退出登录</div>
    </div>

    <!-- 弹窗 -->
    <div class="medium" v-show="this.confirm">
      <div class="medium-header">
        <img src="../assets/感叹号.png" alt />
        <p>上传失败</p>
      </div>
      <div class="medium-footer">
        <p @click="change1">确认</p>
      </div>
    </div>

    <div class="medium" v-show="this.phone">
      <div class="medium-header">
        <img src="../assets/感叹号.png" alt />
        <p>请在手机APP中设置</p>
      </div>
      <div class="medium-footer">
        <p @click="change1">确认</p>
      </div>
    </div>

    <div class="popub" v-show="this.ended">
      <div class="popub-header">
        <img src="../assets/感叹号 (1).png" alt />
        <h2>是否退出登录</h2>
      </div>
      <div class="popub-footer">
        <button @click="change1" class="wite">再等等</button>
        <router-link to="/My">
          <span>
            <button>退出登录</button>
          </span>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AccountInformation",
  data() {
    return {
      ended: false,
      confirm: false,
      phone: false,
      username: ""
    };
  },
  beforeRouteEnter(to, from, next) {
    next(vm => {
      vm.getName(to.params.username);
    });
  },
  methods: {
    getName(username) {
      this.username = username;
    },
    change() {
      this.ended = true;
    },
    change1() {
      this.ended = false;
      this.confirm = false;
      this.phone = false;
    },
    change2() {
      this.confirm = true;
    },
    change3() {
      this.phone = true;
    }
  }
};
</script>


<style scoped>
.Account-information {
  width: 95%;
  margin: 0 auto;
  /* margin-left: 0.5rem; */
}
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
}
.content h2 {
  font-size: 0.6rem;
  color: #333;
  font-weight: 500;
  display: flex;
  align-items: center;
  margin-left: 0.7em;
}
.content div:nth-child(1) {
  background: #fff;
  margin-top: 0.1rem;
  width: 100%;
  height: 3.1rem;
  display: flex;
  justify-content: space-between;
}
.upload {
  display: block;
  position: absolute;
  opacity: 0;
}
.user span img {
  width: 0.7rem;
  height: 0.7rem;
  margin-top: 1rem;
  margin-right: 0.3rem;
  /* flex: 1; */
}
.upload-img img {
  width: 2rem;
  height: 2rem;
  border-radius: 50%;
  vertical-align: middle;
  margin-top: 0.5rem;
  margin-right: 0.3rem;
}
.upload-img span img {
  width: 0.7rem;
  height: 0.7rem;
  margin-top: 1.2rem;
}
.content div:nth-child(2) {
  background: #fff;
  /* margin-top: 1rem; */
  border-top: 1px solid #eee;
  height: 3.1rem;
  display: flex;
  justify-content: space-between;
}
.content div:nth-child(3) {
  background: #fff;
  /* margin-top: 1rem; */
  border-top: 1px solid #eee;
  height: 3.1rem;
  display: flex;
  justify-content: space-between;
}
.user p {
  text-align: left;
  margin-top: 1rem;
  margin-right: 1rem;
  font-size: 0.7rem;
  color: #999;
  font-weight: 100;
  font-family: Arial;
}
.content div:nth-child(4) {
  padding: 0.4rem;
  font-size: 0.5rem;
  color: #666;
}
.phone {
  display: flex;
  background: #fff;
  height: 3.1rem;
}
.phone div:nth-child(1) {
  margin-left: 1rem;
  flex: 3;
  margin-right: 12rem;
  margin-top: 1rem;
}
.phone div:nth-child(2) {
  flex: 1;
  position: absolute;
  left: 14.8rem;
}
.phone div:nth-child(1) img {
  width: 1rem;
  height: 1rem;
  margin-left: -0.5rem;
}
.phone h2 {
  margin-top: -2rem;
  position: absolute;
  top: 16.6rem;
  left: 2rem;
}
.content div:nth-child(6) {
  padding: 0.4rem;
  font-size: 0.5rem;
  color: #666;
}
.content div:nth-child(7) {
  background: #fff;
  /* margin-top: 1rem; */
  border-top: 1px solid #eee;
  height: 3.1rem;
  display: flex;
  justify-content: space-between;
}
.content div:nth-child(8) {
  width: 96%;
  margin: 1.3rem auto 0;
  line-height: 1.5rem;
  border-radius: 5px;
  text-align: center;
  background: #d8584a;
  font-size: 0.6rem;
  color: #fff;
}

.popub {
  width: 94%;
  background: #fff;
  padding: 17px;
  position: absolute;
  top: 20%;
  left: 3%;
  z-index: 1000;
  border-radius: 5px;
  transition: all 1s;
  animation: bounceIn 0.6s;
}
.popub-header img {
  position: relative;
  width: 3rem;
  height: 3rem;
  border-radius: 50%;
  top: 0.5rem;
  left: 5.5rem;
}
.popub-header h2 {
  width: 100%;
  text-align: center;
  font-size: 30px;
  color: #575757;
  font-weight: 500;
  margin: 25px 0;
}
.popub-footer {
  width: 100%;
  text-align: center;
}
.popub-footer button {
  display: inline-block;
  padding: 0.4rem 1rem;
  border-radius: 5px;
  font-size: 0.6rem;
  color: #fff;
  letter-spacing: 1px;
  margin-top: 26px;
}
.popub-footer .wite {
  background: #c1c1c1;
  margin-right: 0.4rem;
}
.popub-footer span button {
  background: #dd6b55;
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
