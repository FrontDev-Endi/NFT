<script setup>
import Slayder from "./Ex-slayder.vue";
</script>

<template>
  <div class="explore">
    <div class="title">
      <h1>Explore By Categories</h1>
      <svg
        width="110"
        height="110"
        viewBox="0 0 110 110"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <circle cx="55" cy="55" r="55" fill="#8613A5" />
      </svg>
    </div>
    <Slayder />
  </div>
</template>

<style lang="scss" scoped>
.explore {
  width: 100%;
  height: 926px;
  background: #251928;
  .title {
    display: flex;
    justify-content: center;
    padding-top: 80px;
    svg {
      border-radius: 100%;
      fill: #8613a5;
      position: absolute;
      margin-left: -650px;
      margin-top: 6px;
    }
    h1 {
      font-family: "Oxanium", sans-serif;
      margin-top: 25px;
      z-index: 1;
      font-weight: 700;
      font-size: 64px;
      color: #f5fbf2;
    }
  }
}

@media (max-width: 1000px) {
  .explore {
    .title {
      h1 {
        font-size: 50px;
      }
      svg {
        margin-left: -467px;
      }
    }
  }
}

@media (max-width: 600px) {
  .explore {
    .title {
      h1 {
        font-size: 40px;
      }
      svg {
        margin-left: -367px;
        margin-top: -6px;
      }
    }
  }
}

@media (max-width: 500px) {
  .explore {
    .title {
      h1 {
        font-size: 30px;
      }
      svg {
        margin-left: -267px;
        margin-top: 5px;
        width: 80px;
        height: 80px;
      }
    }
  }
}

@media (max-width: 425px) {
  .explore {
    height: 826px;
  }
}
</style>
