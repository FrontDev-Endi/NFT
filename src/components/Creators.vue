<script setup>
  import Collection from "./Сollection.vue";
</script>

<template>
  <div class="creators">
    <div class="title wow animate__animated animate__fadeIn">
      <h1>Top Creators</h1>
      <svg
        width="110"
        height="110"
        viewBox="0 0 110 110"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <circle cx="55" cy="55" r="55" fill="#E03054" />
      </svg>
    </div>
    <Collection />
  </div>
</template>

<style lang="scss" scoped>
.creators {
  width: 100%;
  margin-top: 104px;
  .title {
    display: flex;
    justify-content: center;
    svg {
      border-radius: 100%;
      fill: #e03054;
      position: absolute;
      margin-left: -350px;
      margin-top: 6px;
    }
    h1 {
      font-family: "Oxanium", sans-serif;
      font-weight: 700;
      font-size: 64px;
      line-height: 2.03125;
      color: #f5fbf2;
      z-index: 1;
    }
  }
}

@media (max-width: 1000px) {
  .creators {
    .title {
      h1 {
        font-size: 50px;
      }
      svg {
        margin-left: -250px;
        margin-top: -12px;
      }
    }
  }
}

@media (max-width: 500px) {
  .creators {
    .title {
      h1 {
        font-size: 30px;
      }
      svg {
        margin-left: -150px;
        margin-top: -12px;
        width: 80px;
      }
    }
  }
}
</style>
