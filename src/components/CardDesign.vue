<template>
  <swiper
    :effect="'coverflow'"
    :grabCursor="true"
    :centeredSlides="true"
    :slidesPerView="'auto'"
    :initialSlide="'2'"
    :loop="true"
    :coverflowEffect="{
      rotate: 0,
      stretch: 0,
      depth: 100,
      modifier: 2,
      slideShadows: true,
    }"
    :pagination="true"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide v-for="(foto, $index) in img" :key="$index">
        <img :src="'/assets/img/'+foto.source" />
        <h3>{{foto.name}}</h3>
        <p>{{foto.desc}}</p>
    </swiper-slide>

  </swiper>
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/effect-coverflow";
import "swiper/css/pagination";

// import required modules
import { EffectCoverflow, Pagination } from "swiper";

export default {
  data() {
    return {
      img: []
    }
  },
  mounted() {
    fetch("/assets/dataimg.json")
    .then(res => res.json())
    .then(res => {
      this.img = res
    })
  },
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [EffectCoverflow, Pagination],
    };
  },
};
</script>

<style>
    .swiper {
    width: 100%;
    padding-top: 50px;
    padding-bottom: 50px;
    }

    .swiper-slide {
    background-position: center;
    background-size: cover;
    width: 300px;
    height: 300px;
    margin-bottom: 66px;
    }

    .swiper-slide h3 {
      font-size: 24px;
      color: #304025;
      margin: 18px 0 0 0;
      text-align: center;
    }

    .swiper-slide p {
      font-size: 16px;
      font-style: italic;
      color: #304025;
      margin-bottom: 18px;
      text-align: center;
    }

    .swiper-slide img {
    border-radius: 5px;
    display: block;
    max-width: 100%;
    }
</style>
