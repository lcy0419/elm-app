<template>
  <div id="app">
    <!-- <My /> -->
    <keep-alive>
      <router-view></router-view>
    </keep-alive>
  </div>
</template>
<script>
import My from "./components/My";
export default {
  data() {
    return {};
  },
  components: {
    My
  }
};
</script>
<style>
html {
  font-size: 100px;
  background: #99999910;
}
.left {
  float: left;
}
.right {
  float: right;
}
.clear {
  overflow: hidden;
}
@media screen and (max-width: 320px) {
  html {
    font-size: 12px;
  }
}
@media screen and (min-width: 320px) and (max-width: 360px) {
  html {
    font-size: 20px;
  }
}
@media screen and (min-width: 360px) and (max-width: 375px) {
  html {
    font-size: 22px;
  }
}
@media screen and (min-width: 375px) and (max-width: 411px) {
  html {
    font-size: 23px;
  }
}
@media screen and (min-width: 411px) and (max-width: 414px) {
  html {
    font-size: 25px;
  }
}
@media screen and (min-width: 411px) and (max-width: 768px) {
  html {
    font-size: 25.5px;
  }
}
@media screen and (min-width: 768px) and (max-width: 1024px) {
  html {
    font-size: 48px;
  }
}
@media screen and (min-width: 1024) {
  html {
    font-size: 64px;
  }
}
* {
  padding: 0;
  margin: 0;
  list-style: none;
  font-style: normal;
  text-decoration: none;
  border: none;
  color: #333;
  font-weight: 400;
  font-family: Microsoft Yahei;
  box-sizing: border-box;
  -webkit-tap-highlight-color: transparent;
  -webkit-font-smoothing: antialiased;
}
</style>
