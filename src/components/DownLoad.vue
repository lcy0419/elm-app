<template>
  <div class="down-load">
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
        <span class="you">下载</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <img src="../assets/饿了么.jpg" alt />
      <p>下载饿了么APP</p>
      <div class="down" @click="change">下载</div>
    </div>

    <!-- 弹窗 -->
    <div class="popub" v-show="this.ended">
      <div class="popub-header">
        <img src="../assets/感叹号.png" alt />
        <p>IOS用户请前往AppStore下载</p>
      </div>
      <div class="popub-footer">
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
      ended: false
    };
  },
  methods: {
    change() {
      this.ended = true;
    },
    change1() {
      this.ended = false;
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
}
.content img {
  border-radius: 1rem;
  margin-top: 1rem;
  margin-left: 4.3rem;
}
.content p {
  text-align: center;
  font-size: 0.8rem;
  color: #666;
  margin-bottom: 1rem;
}
.content .down {
  background-color: #4cd964;
  font-size: 0.7rem;
  color: #fff;
  text-align: center;
  margin: 0 0.7rem;
  line-height: 1.8rem;
  border-radius: 0.2rem;
  margin-top: 0.5rem;
}
.popub {
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
.popub-header img {
  position: relative;
  width: 3rem;
  height: 3rem;
  border-radius: 50%;
  top: 0.5rem;
  left: 4.5rem;
}
.popub-header p {
  font-size: 0.7rem;
  color: #333;
  line-height: 0.9rem;
  text-align: center;
  margin-top: 0.8rem;
  padding: 0 0.4rem;
}
.popub-footer {
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
.popub-footer p {
  color: #fff;
}
</style>
