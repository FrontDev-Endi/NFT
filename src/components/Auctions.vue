<script setup>
import SlayderLive from "./Slaederlove.vue";
</script>

<template>
  <div class="eff"></div>
  <div class="auctions">
    <div class="title wow animate__animated animate__fadeIn">
      <svg
        width="110"
        height="110"
        viewBox="0 0 110 110"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <circle cx="55" cy="55" r="55" fill="#8613A5" />
      </svg>
      <h1>Live Auctions</h1>
    </div>
    <SlayderLive />
  </div>
</template>
<style lang="scss" scoped>
.eff{
  position: absolute;
  width: 228px;
  height: 167px;
  margin-left: 210px;
  margin-top: 43px;
  background: rgba(231, 178, 38, 0.7);
  filter: blur(450px);
}
.auctions {
  margin-top: 104px;
  height: 1233px;
  width: 100%;
  background: #251928;
  .title{
    display: flex;
    justify-content: center;
    padding-top: 80px;
    h1{
      padding-right: 20px;
      font-family: 'Oxanium', sans-serif;
      font-weight: 700;
      font-size: 64px;
      line-height: 96px;
      line-height: 1.5;
      color: var(--white-two);
      z-index: 1;
    }
    svg{
      position: absolute;
      margin-left: -400px;
      margin-top: -10px;

    }
  }
}

@media (max-width: 1000px) {
  .auctions {
    .title {
      h1 {
        font-size: 50px;
      }
      svg {
        margin-left: -300px;
        margin-top: -20px;
      }
    }
  }
}

@media (max-width: 600px) {
  .auctions {
    height: 933px;
  }
}

@media (max-width: 425px) {
  .eff{
    margin-left: 0px;
  }
}
</style>
