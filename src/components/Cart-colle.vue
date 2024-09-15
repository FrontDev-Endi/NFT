<script setup>
defineProps({
  imageUrl: String,
});
</script>

<template>
  <div class="cart">
    <div class="logo">
      <img :src="imageUrl" alt="ava" />
    </div>
    <div class="info">
      <h1>Wzard Dee</h1>
      <p>4.89 ETH</p>
    </div>
    <div class="linea"></div>
    <div class="items">
      <h1>33</h1>
      <p>items</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.cart {
  width: 608px;
  height: 156px;
  box-shadow: inset 2px 0 0 0 #e03054;
  background: #302034;
  display: flex;
  margin-bottom: 56px;
  .logo {
    img {
      width: 104px;
      height: 104px;
      margin: 26px 24px 26px 29px;
    }
  }
  .info {
    margin-top: 42px;
    h1 {
      font-family: "Oxanium", sans-serif;
      font-weight: 600;
      font-size: 32px;
      line-height: 1.10788;
      letter-spacing: 0.05em;
      color: #f5fbf2;
    }
    p {
      font-family: "Work Sans", sans-serif;
      font-weight: 500;
      font-size: 24px;
      line-height: 1.5;
      color: #bdaac1;
    }
  }
  .linea {
    margin-left: 45px;
    margin-top: 75px;
    border: 2px solid #49374e;
    width: 100px;
    height: 0px;
    transform: rotate(-90deg);
  }
  .items {
    margin-top: 39px;
    h1 {
      font-family: "Oxanium", sans-serif;
      margin-left: 17px;
      font-weight: 700;
      font-size: 32px;
      line-height: 1.10788;
      letter-spacing: 0.05em;
      color: #f5fbf2;
    }
    p {
      font-family: "Work Sans", sans-serif;
      margin-top: 6px;
      margin-left: 5px;
      font-weight: 500;
      font-size: 24px;
      line-height: 1.5;
      color: #908294;
    }
  }
}

@media (max-width: 1380px) {
  .cart {
    width: 508px;
    height: 125px;
    .logo img {
      width: 84px;
      height: 84px;
      margin-top: 23px;
    }
    .info {
      h1 {
        font-size: 28px;
      }
      p {
        font-size: 20px;
      }
    }
    .linea {
      margin-left: 20px;
      margin-top: 61px;
    }
    .items {
      h1 {
        margin-left: 0;
      }
      p{
        margin-top: 0px;
        margin-left: -12px;
      }
    }
  }
}

@media (max-width: 1120px) {
  .cart {
    width: 475px;
    height: 125px;
    .logo img {
      width: 74px;
      height: 74px;
      margin-top: 23px;
    }
    .info {
      h1 {
        font-size: 24px;
      }
      p {
        font-size: 18px;
      }
    }
    .linea {
      margin-left: 13px;
      margin-top: 61px;
    }
    .items {
      h1 {
        margin-left: 0;
      }
      p{
        margin-top: 0px;
        margin-left: -12px;
      }
    }
  }
}

@media (max-width: 600px) {
  .cart {
    width: 375px;
    height: 125px;
    .logo img {
      width: 60px;
      // height: 60px;
      margin-top: 23px;
      margin-left: 13px;
    }
    .info {
      margin-top: 37px;
      h1 {
        font-size: 20px;
      }
      p {
        font-size: 18px;
      }
    }
    .linea {
      margin-left: 0px;
      margin-top: 61px;
    }
    .items {
      margin-top: 35px;
      h1 {
        margin-left: -12px;
      }
      p{
        margin-top: 0px;
        margin-left: -25px;
      }
    }
  }
}
</style>
