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
        <span class="zhong">编辑地址</span>
        <span class="you" @click="edit1" v-show="ended">{{text}}</span>
        <span class="you" @click="edit2" v-show="!ended">{{text}}</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <router-link to="/AddAddress">
        <div>
          <span>新增地址</span>
          <span>
            <img src="../assets/right.png" alt />
          </span>
        </div>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "DownLoad",
  data() {
    return {
      text: "编辑",
      ended: true
    };
  },
  methods: {
    edit1() {
      this.text = "完成";
      this.ended = false;
    },
    edit2() {
      this.text = "编辑";
      this.ended = true;
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
  display: flex;
  justify-content: space-between;
  line-height: 1.95rem;
}
.header-top span {
  color: #ffffff;
}
.zuo {
  margin-left: 0.3rem;
}
.zhong {
  font-size: 0.8rem;
  color: #fff;
  text-align: center;
  font-weight: 700;
}
.you {
  right: 0.4rem;
  font-size: 0.7rem;
  color: #fff;
  margin-right: 0.3rem;
}
.content {
  margin-top: 2.5rem;
}
.content div {
  margin-top: 0.4rem;
  background: #fff;
  padding: 0.2rem 0.4rem;
  border-top: 1px solid #d9d9d9;
  display: flex;
  justify-content: space-between;
}
.content span {
  display: block;
  font-size: 0.7rem;
  color: #333;
  line-height: 1.4rem;
}
</style>
