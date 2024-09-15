<script setup>
defineProps({
  Icon: String,
  Text: String,
  Alt: String,
});
</script>

<template>
  <div class="cart">
    <div class="img">
      <img :src="Icon" :alt="Alt" />
    </div>
    <h1>{{ Text }}</h1>
  </div>
</template>

<style lang="scss" scoped>
.cart {
  .img {
    text-align: center;
    img {
      padding-bottom: 32px;
    }
  }
  h1 {
    font-family: "Work Sans", sans-serif;
    font-weight: 600;
    font-size: 24px;
    text-align: center;
    text-transform: capitalize;
    color: #ffce4e;
    padding-bottom: 32px;
  }
}

@media (max-width: 1462px) {
  .cart {
    .img {
      img {
        width: 106px;
        height: 106px;
      }
    }
    h1 {
      font-size: 20px;
    }
  }
}

@media (max-width: 1180px) {
  .cart {
    .img {
      width: 106px;
      height: 106px;
      margin-left: auto;
      margin-right: auto;
      img {
      }
    }
    h1{
      font-size: 17px;
    }
  }
}
</style>
