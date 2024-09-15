<script>
import Slayder from "./Pop-slayd.vue";

import { ref } from "vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay } from "swiper/modules";
import "swiper/css";

export default {
  components: {
    Slayder,
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiper = (swiper) => {};
    const onSlideChange = () => {};
    const prev = ref(null);
    const next = ref(null);
    return {
      modules: [Autoplay],
      prev,
      next,
      Swiper,
      onSwiper,
      onSlideChange,
    };
  },
};
</script>

<!-- two scroll -->

<template>
  <swiper
    :modules="modules"
    class="swiper slayder animate__animated animate__flipInX wow"
    :space-between="50"
    :slides-per-view="1"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
    :autoplay="{
      delay: 1000,
      disableOnInteraction: false,
    }"
    :breakpoints="{
      1599:{
        slidesPerView: 1,
      },
      1600: {
        slidesPerView: 2,
      },
      1750: {
        slidesPerView: 3,
      }
    }"
  >
    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%202.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%203.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%204.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%202.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%203.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%204.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%202.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%203.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%204.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%202.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%203.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%204.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%202.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%203.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%204.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%202.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%203.png" />
    </swiper-slide>

    <swiper-slide class="swiper-slide">
      <Slayder imagePop="/src/assets/img/image%204.png" />
    </swiper-slide>
  </swiper>
</template>

<style lang="scss" scoped>
.slayder {
  display: flex;
  width: 88%;
}
.swiper-slide {
  justify-content: center;
}
@media (max-width: 1740px) {
  .slayder {
    width: 66%;
    display: flex;
    justify-content: center;
  }
}

@media (max-width: 1700px) {
  .slayder {
    width: 66%;
    display: flex;
    justify-content: center;
  }
}
@media (max-width: 1600px) {
  .slayder{
    width: 525px;
  }
}
@media (max-width: 600px) {
  .slayder{
    width: 343px;
  }
}
</style>
