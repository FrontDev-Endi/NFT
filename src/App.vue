<script setup>
import Header from "./components/Header.vue";
import Sponsors from "./components/Sponsors.vue";
import Auctions from "./components/Auctions.vue";
import Works from "./components/Works.vue";
import Popular from "./components/Popular-collections.vue";
import Explore from "./components/Explore.vue";
import Creators from "./components/Creators.vue";
import Email from "./components/Email.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  
  <Header />
  <Sponsors />
  <Auctions />
  <Works />
  <Popular />
  <Explore />
  <Creators />
  <Email />
  <Footer />
</template>

<style scoped lang="scss">

span.swiper-pagination-bullet.swiper-pagination-bullet-active {
  background: #ffce4e;
}
@media (max-width: 1662px) {
  .box{
    margin-left: 52.2%;
  }
}
</style>
