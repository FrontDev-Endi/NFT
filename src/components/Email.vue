<script setup>
  import Inputemail from "./Inputemail.vue";
</script>

<template>
  <div class="email wow animate__animated animate__flipInX">
    <h1>Ready for Next NFT Drop?</h1>
    <Inputemail />
  </div>
</template>

<style lang="scss" scoped>
.email {
  margin-top: 117px;
  h1 {
    font-family: "Oxanium", sans-serif;
    font-weight: 700;
    font-size: 64px;
    text-align: center;
    color: #f5fbf2;
  }
}
@media (max-width: 1380px) {
  .email {
    h1 {
      font-size: 54px;
    }
  }
}

@media (max-width: 1000px) {
  .email {
    h1 {
      font-size: 50px;
    }
  }
}

@media (max-width: 768px) {
  .email {
    h1 {
      font-size: 40px;
    }
  }
}

@media (max-width: 600px) {
  .email {
    h1 {
      font-size: 30px;
    }
  }
}
</style>
