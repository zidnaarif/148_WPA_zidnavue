<template>
<div class="review-card">
  <swiper
    :effect="'cards'"
    :grabCursor="true"
    :modules="modules"
    :loop="true"
    class="mySwiper"
  >
    <swiper-slide v-for="(data, $index) in review" :key="$index">
      <div class="testi">
        <div class="quote">
          <img src="/assets/img/quote.png" alt="">
        </div>
        <div class="content">
          <p>{{data.message}}</p>
          <div class="detail">
            <div class="imgbox">
              <img :src="`${data.avatar}`" alt="">
            </div>
            <div class="profile">
              <h4>{{data.name}}</h4>
              <span>{{data.location}}</span>
            </div>
          </div>
        </div>
      </div>
    </swiper-slide>

  </swiper>

</div>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/effect-cards";
import "swiper/css/autoplay";

// import required modules
import { EffectCards } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      review: []
    }
  },
  mounted() {
    fetch("https://testimonialapi.toolcarton.com/api")
    .then (res => res.json())
    .then (res => {
      this.review = res.sort((a,b) => a.rating - b.rating)
    })
  },
  setup() {
    return {
      modules: [EffectCards],
    };
  },
};
</script>

<style>
  .review-card .swiper {
    width: 260px;
    height: 400px;
  }

  .review-card .swiper-slide {
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 18px;
    font-size: 22px;
    font-weight: bold;
    color: rgb(26, 26, 26);
  }

  .review-card .swiper-slide:nth-child(1n) {
    background-color: rgb(255, 255, 255);
  }

  .testi {
    margin: 0px 36px 10px 36px;
  }

  .testi .quote {
    position: absolute;
    right: 20px;
  }

  .testi .quote img {
    max-width: 34px;
  }

  .testi .content {
    margin-top: 40px;
  }

  .testi .content p {
    color: #304025;
    font-weight: lighter;
    font-style: italic;
    text-align: left;
    font-size: 12px;
  }

  .testi .detail {
    display: flex;
  }

  .testi .detail .imgbox {
    position: relative;
    border-radius: 50%;
    overflow: hidden;
    margin-top: 10px;
    margin-right: 10px;
    max-width: 60px;
  }

  .testi .detail .imgbox {
    object-fit: cover;
  }

  .testi .profile {
    margin-left: 5px;
  }

  .testi .profile h4 {
    color: #304025;
    font-size: 14px;
    font-weight: bold;
    margin-top: 20px;
    margin-bottom: -10px;
    padding: 0;
  }
  
  .testi .profile span {
    font-size: 12px;
    font-weight: normal;
    color: #304025;
  }

</style>