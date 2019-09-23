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
        <span class="you">修改用户名</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <input type="text" placeholder="输入用户名" v-model="username" />
      <p>用户名只能修改一次（5-24字符之间）</p>
    </div>

    <router-link :to="{name:'AccountInformation',params:{username:username}}">
      <div class="footer">
        <button>确认修改</button>
      </div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: "DownLoad",
  data() {
    return {
      ended: false,
      username: "",
      password: ""
    };
  },
  created() {
    this.getPassword;
  },
  methods: {
    change() {
      this.ended = true;
    },
    change1() {
      this.ended = false;
    },
    getPassword() {
      this.$axios.post(`https://elm.cangdu.org/v2/changepassword`).then(res => {
        console.log(res);
        this.password = res;
      });
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
  margin-top: 2rem;
  /* margin-left: 0rem; */
}
.content input {
  background: none;
  width: 13.6rem;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0.2rem 0.1rem;
  line-height: 1.2rem;
  font-size: 0.7rem;
  display: block;
  text-rendering: auto;
  margin-left: 0.6rem;
  padding-left: 0.5rem;
  margin-top: 2.5rem;
}
.content p {
  width: 100%;
  font-size: 0.4rem;
  color: #666;
  padding: 0.4rem 0 1rem;
  margin-left: 0.6rem;
}
.footer button {
  display: block;
  width: 15.2rem;
  background: #3190e8;
  line-height: 2rem;
  font-size: 0.7rem;
  color: #fff;
  opacity: 0.8;
  margin-left: -0.4rem;
  transition: all 1s;
}
</style>
