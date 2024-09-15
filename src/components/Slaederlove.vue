<script>
import Slayd from "./Slayd.vue";

import { ref } from "vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import { Navigation } from "swiper/modules";
import "swiper/css/navigation";

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
      modules: [Navigation],
      prev,
      next,
      Swiper,
      onSwiper,
      onSlideChange,
    };
  },
};
</script>

<!-- one scroll -->

<template>
  <div ref="prev" class="swiper-button-prev"></div>
  <div ref="next" class="swiper-button-next"></div>
  <swiper
    :navigation="{
      prevEl: prev,
      nextEl: next,
    }"
    :modules="modules"
    class="swiper slayder animate__animated animate__bounceInLeft wow"
    :slides-per-view="1"
    :space-between="50"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
    :breakpoints="{
      1430: {
        slidesPerView: 2,
      },
      1606: {
        slidesPerView: 3,
      },
    }"
  >
    <swiper-slide class="swiper-slide">
      <Slayd image-url="/src/assets/img/image%201.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="/src/assets/img/image%2023.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="/src/assets/img/image%203.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="/src/assets/img/image%201.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="/src/assets/img/image%2023.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="/src/assets/img/image%203.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="/src/assets/img/image%201.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="/src/assets/img/image%2023.png" />
    </swiper-slide>
    <swiper-slide class="swiper-slide">
      <Slayd image-url="/src/assets/img/image%203.png" />
    </swiper-slide>
  </swiper>
  <!-- <div class="view-all">
    <button class="btn-all">View All</button>
    
  </div> -->
</template>

<style lang="scss" scoped>
.swiper-button-prev {
  // position: relative;
  background-image: url(../assets/img/arrow-next.png);
  transform: rotate(180deg);
  width: 54px;
  height: 54px;
  margin-top: 1050px;
  margin-left: 76%;
}
.swiper-button-next {
  // position: relative;
  background-image: url(../assets/img/arrow-next.png);
  width: 54px;
  height: 54px;
  margin-top: 1050px;
  margin-right: 15%;
}
.swiper-button-next:after,
.swiper-rtl .swiper-button-prev:after {
  content: none;
}
.swiper-button-prev:after,
.swiper-rtl .swiper-button-next:after {
  content: none;
}
.swiper-wrapper {
  min-width: 0;
}
.slayder {
  display: flex;
  justify-content: center;
  margin-top: 90px;
  margin-left: auto;
  height: 700px;
  width: 1569px;
  z-index: 10;
  .swiper-slide {
    width: 495px;
    height: 691px;
    padding-top: 12px;
  }
}

@media (max-width: 1606px) {
  .slayder {
    width: 70%;
  }
}
@media (max-width: 1454px) {
  .swiper-button-prev {
    margin-left: 73%;
  }
}
@media (max-width: 1430px) {
  .slayder {
    width: 495px;
  }
}
@media (max-width: 1170px) {
  .swiper-button-prev {
    margin-top: 1900px;
  }
  .swiper-button-next {
    margin-top: 1900px;
  }
}
@media (max-width: 1000px) {
  .swiper-button-prev {
    margin-top: 1850px;
  }
  .swiper-button-next {
    margin-top: 1850px;
    margin-right: 12%;
  }
}
@media (max-width: 900px) {
  .swiper-button-next {
    margin-top: 1800px;
  }
  .swiper-button-prev {
    margin-top: 1800px;
  }
}
@media (max-width: 770px) {
  .swiper-button-prev {
    margin-top: 1050px;
    margin-left: 66%;
  }
  .swiper-button-next {
    margin-top: 1050px;
    margin-right: 15%;
  }
}
@media (max-width: 700px) {
  .swiper-button-prev {
    margin-top: 1050px;
    margin-left: 60%;
  }
  .swiper-button-next {
    margin-top: 1050px;
    margin-right: 17%;
  }
}
@media (max-width: 600px) {
  .slayder {
    width: 360px;
  }
  .swiper-button-prev {
    margin-top: 1000px;
    margin-left: 60%;
  }
  .swiper-button-next {
    margin-top: 1000px;
    margin-right: 17%;
  }
}
@media (max-width: 550px) {
  .swiper-button-prev {
    margin-top: 1000px;
    margin-left: 55%;
  }
  .swiper-button-next {
    margin-top: 1000px;
    margin-right: 17%;
  }
}

@media (max-width: 500px) {
  .swiper-button-prev {
    margin-top: 850px;
    margin-left: 55%;
  }
  .swiper-button-next {
    margin-top: 850px;
    margin-right: 17%;
  }
}
</style>
