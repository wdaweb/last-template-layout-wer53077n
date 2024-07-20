<template>
  <swiper
    :spaceBetween="30"
    :effect="'fade'"
    :navigation="true"
    :pagination="{
      clickable: true,
    }"
    :modules="modules"
    :autoplay="{
      delay: 1000,
      disableOnInteraction: true,
    }"
    class="mySwiper"
  >
    <swiper-slide
      ><img src="https://picsum.photos/1900/600/?random=1" /></swiper-slide
    ><swiper-slide
      ><img src="https://picsum.photos/1900/600/?random=2" /></swiper-slide
    ><swiper-slide
      ><img src="https://picsum.photos/1900/600/?random=3" /></swiper-slide
    ><swiper-slide
      ><img src="https://picsum.photos/1900/600/?random=4"
    /></swiper-slide>
  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/effect-fade";
import "swiper/css/navigation";
import "swiper/css/pagination";

// import required modules
import { EffectFade, Navigation, Pagination } from "swiper/modules";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [EffectFade, Navigation, Pagination],
    };
  },
};
</script>
