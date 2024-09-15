<script setup>
import Slyder from "./Slyder-popular.vue";
</script>

<template>
  <div class="popular">
    <div class="effect"></div>
    <div class="title">
      <svg
        width="110"
        height="110"
        viewBox="0 0 110 110"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <circle cx="55" cy="55" r="55" fill="#E03054" />
      </svg>
      <h1>Popular Collections</h1>
    </div>
    <Slyder />
  </div>
</template>

<style lang="scss" scoped>
.effect {
  width: 180px;
  height: 167px;
  // margin-top: 239px;
  margin-left: 400px;
  filter: blur(150px);
  background: #60e7ce;
}
.popular {
  padding-bottom: 104px;
  .title {
    display: flex;
    text-align: center;
    justify-content: center;
    padding-bottom: 106px;
    h1 {
      font-family: "Oxanium", sans-serif;
      font-weight: 700;
      font-size: 64px;
      line-height: 2.03125;
      color: #fff;
      z-index: 1;
    }
    svg {
      position: absolute;
      z-index: -1;
      margin-left: -550px;
      margin-top: 6px;
    }
  }
}

@media (max-width: 1000px) {
  .popular {
    .title {
      h1 {
        font-size: 50px;
      }
      svg {
        margin-left: -430px;
        margin-top: -5px;
      }
    }
  }
}

@media (max-width: 600px) {
  .effect {
    width: 180px;
    height: 167px;
    // margin-top: 239px;
    margin-left: 300px;
    filter: blur(150px);
    background: #60e7ce;
  }
  .popular {
    .title {
      h1 {
        font-size: 40px;
      }
      svg {
        margin-left: -330px;
        margin-top: -5px;
        width: 100px;
        height: 100px;
      }
    }
  }
}

@media (max-width: 500px) {
  .popular {
    .effect {
      margin-left: 100px;
    }
    .title {
      h1 {
        font-size: 30px;
      }
      svg {
        margin-left: -230px;
        margin-top: -5px;
        width: 80px;
        height: 80px;
      }
    }
  }
}
</style>
