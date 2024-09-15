<script>
import Slayd from "./Ex-slayd.vue";

import { ref } from "vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Pagination } from "swiper/modules";
import "swiper/css";
import "swiper/css/pagination";

export default {
  components: {
    Slayd,
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiper = (swiper) => {};
    const onSlideChange = () => {};
    const prev = ref(null);
    const next = ref(null);
    return {
      modules: [Pagination],
      prev,
      next,
      Swiper,
      onSwiper,
      onSlideChange,
    };
  },
};
</script>

<!-- three scroll -->

<template>
  <swiper
    :modules="modules"
    class="swiper slayder animate__animated animate__fadeInUpBig wow"
    :slides-per-view="1"
    :space-between="50"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
    :pagination="{
      clickable: true,
    }"
    :breakpoints="{
      1390: {
        slidesPerView: 2,
      },
      1660: {
        slidesPerView: 3,
      }
    }"
  >
    <swiper-slide class="swiper-slide">
      <Slayd image-url="./assets/img/image%205.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="./assets/img/image%2024.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="./assets/img/image%2025.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="./assets/img/image%205.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="./assets/img/image%2024.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="./assets/img/image%2025.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="./assets/img/image%205.png" />
    </swiper-slide>
  </swiper>
</template>

<style lang="scss" scoped>
.slayder {
  display: flex;
  width: 1329px;
  height: 550px;
  margin-left: auto;
  margin-right: auto;
  margin-top: 84px;
}
@media (max-width: 1660px) {
  .slayder {
    width: 70%;
  }
}
@media (max-width: 1390px) {
  .slayder {
    width: 415px;
  }
}
@media (max-width: 500px) {
  .slayder {
    width: 315px;
  }
}
</style>
