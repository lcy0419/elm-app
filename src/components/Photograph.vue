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
        <span class="you">教我拍大片</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->
    <div class="content">
      <p>
        <img src="../assets/fish.jpeg" alt />
        "## 1.清晰拍照时持稳手机，避免出现大幅度晃动。将焦点对准食物本身，锁焦后、点击快门。"
        <br />
        <br />
        <br />
        <img src="../assets/fish2.jpeg" alt />
        "## 2.光线尽量选择明亮。柔和的光线，避免强光直射；拍摄时避免身体或器物的阴影遮住器物本身，有条件时可以用小型手电进行补光，以提高食物质感"
        <br />
        <br />
        <br />
        <img src="../assets/fish3.jpeg" alt />
        "## 3.构图可以选择通用的三分构图法或中心构图法，如果是拍摄整体食物时，需要考虑食物的完整性；如果拍摄特写时，需要将细节体现清楚。"
        <br />
        <br />
        <br />
        <img src="../assets/fish4.jpeg" alt />
        "## 4.角度可以选择45度拍摄、90度俯拍或者水平拍摄，一切都看你的心情哦~"
        <br />
        <br />
        <br />
        <img src="../assets/fish5.jpeg" alt />
        "## 5.背景可以选择合适的背景拍摄，例如黑色能体现食物蒸腾的热气，白色让食物更有质感，米色更加温馨等；但背景尽量不要太乱，以免影响整体效果。"
        <br />
        <br />
        <br />
        <img src="../assets/fish6.jpeg" alt />
        "## 6.细节 餐具的搭配使用、人物的烘托、道具的陪衬等都能使食物更具诱惑力，照片更有氛围。"
        <br />
        <br />
        <br />
      </p>
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
  margin-top: 1.8rem;
}
.content p {
  font-style: normal;
  text-decoration: none;
  border: none;
  color: #333;
  font-weight: 400;
  font-size: 0.65rem;
}
</style>
