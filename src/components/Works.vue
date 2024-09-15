<script setup>
import List from "./List.vue";
</script>

<template>
  <div class="works wow animate__animated animate__fadeInUp animate__delay-0.9s">
    <h1 class="title">How it works</h1>
    <div class="effect"></div>
    <List />
  </div>
</template>

<style lang="scss" scoped>
.works {
  width: 100%;
  margin-top: 180px;
  .effect {
    width: 172px;
    height: 168px;
    margin: 0 auto;
    margin-top: 40px;
    filter: blur(200px);
    background: #d53d5c;
    
  }
  .title {
    text-align: center;
    font-family: "Oxanium", sans-serif;
    font-weight: 700;
    font-size: 64px;
    color: #f5fbf2;
    z-index: 1;
  }
}

@media (max-width: 500px) {
  .works{
    .title{
      font-size: 42px;
    }
  }
}
</style>
