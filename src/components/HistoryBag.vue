<template>
  <div class="Discount">
    <!-- header -->
    <div class="header">
      <!-- header-top -->
      <div class="header-top">
        <span class="zuo">
          <router-link to="/Discount">
            <a href>
              <img src="../assets/左箭头.png" alt="左箭头" />
            </a>
          </router-link>
        </span>
        <span class="you">历史红包</span>
      </div>
      <!-- header-top-end -->
    </div>
    <!-- header-end -->

    <!-- body -->
    <div class="item2">
      <ul>
        <li v-for="(historybag,index) in historybags" :key="index">
          <div class="content">
            <div>
              <span>￥</span>
              <span>{{historybag.amount}}</span>
              <span>.</span>
              <span>0</span>
              <p>{{historybag.description_map.sum_condition}}</p>
            </div>
            <div class="bag">
              <p>普通红包</p>
              <p>{{historybag.description_map.validity_periods}}</p>
              <p>{{historybag.description_map.phone}}</p>
              <!-- {{historybag.limit_map.restaurant_flavor_ids}} -->
            </div>
            <div>
              <img src="../assets/history.png" alt />
            </div>
          </div>
          <div class="footer">
            <p
              v-if="historybag.limit_map == null? false:true"
            >{{historybag.limit_map.restaurant_flavor_ids}}</p>
          </div>
        </li>
      </ul>
    </div>
    <!-- body-end -->
  </div>
</template>

<script>
export default {
  name: "Discount",
  data() {
    return {
      historybags: []
    };
  },
  created() {
    this.getHistorybag();
  },
  methods: {
    getHistorybag() {
      this.$axios
        .get(
          `https://elm.cangdu.org/promotion/v2/users/1/expired_hongbaos?limit=4&offset=0`
        )
        .then(res => {
          console.log(res.data);
          this.historybags = res.data;
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
  left: 5.5rem;
}
.item2 {
  padding-left: 0.7rem;
  padding-right: 0.7rem;
  margin-top: 3rem;
}
.item2 ul li .content {
  display: flex;
  justify-content: space-between;
  padding: 1rem 0.5rem 0.8rem;
  background: #fff url(../assets/title.png) repeat-x;
  background-size: 0.5rem 0.2rem;
  margin-bottom: 0.5rem;
  border-radius: 0.25rem;
  /* position: relative; */
}
.item2 ul li div:nth-child(1) span:nth-child(1) {
  font-size: 0.75rem;
  color: #ccc;
  font-weight: 700;
}
.item2 ul li div:nth-child(1) span:nth-child(2) {
  font-size: 2rem;
  color: #ccc;
}
.item2 ul li div:nth-child(1) span:nth-child(3) {
  font-size: 1rem;
  color: #ccc;
  font-weight: 700;
}
.item2 ul li div:nth-child(1) span:nth-child(4) {
  font-size: 1rem;
  color: #ccc;
  font-weight: 700;
}
.item2 ul li div:nth-child(1) p {
  font-size: 0.4rem;
  color: #999;
}
.item2 ul li .bag p:nth-child(1) {
  font-size: 0.7rem;
  color: #666;
  margin-left: -0.7rem;
}
.item2 ul li div:nth-child(2) p:nth-child(2) {
  list-style-type: disc;
  margin-left: -0.7rem;
  font-size: 0.4rem;
  color: #999;
}
.item2 ul li div:nth-child(2) p:nth-child(3) {
  list-style-type: disc;
  margin-left: -0.7rem;
  font-size: 0.4rem;
  color: #999;
}

.item2 ul li div:nth-child(3) {
  fill: #ddd;
  width: 3rem;
  height: 3rem;
  top: 0.6rem;
  right: 0.2rem;
  /* position: absolute; */
}
.item2 ul li .footer {
  background-color: rgba(238, 238, 238, 0.212);
  padding: 0.4rem;
  border-bottom-left-radius: 0.25rem;
  border-bottom-right-radius: 0.25rem;
  margin-top: -0.5rem;
}
.item2 ul li .footer p {
  list-style-type: disc;
  font-size: 0.4rem;
  color: #999;
  margin-left: 0.4rem;
}
</style>










