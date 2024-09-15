<template>
  <div class="seti">
    <h4>
      Nec, enim sed lacus, magna pharetra. <br />
      Phasellus tincidunt nulla pharetra <br />
      gravida est.
    </h4>
    <div class="icon">
      <img src="../assets/img/youtube.png" alt="youtube" class="youtube" />
      <img src="../assets/img/twitter.png" alt="twitter" class="twitter" />
      <img src="../assets/img/fais.png" alt="facebook" class="facebook" />
      <img src="../assets/img/google.png" alt="google" class="google" />
    </div>
    <h2>All rights reserved@2021</h2>
  </div>
</template>

<style lang="scss" scoped>
.seti {
  margin-top: 50px;
  margin-left: 51px;
  h4 {
    font-family: "Work Sans", sans-serif;
    padding-bottom: 52px;
    font-weight: 500;
    font-size: 20px;
    line-height: 1.8;
    color: #96839b;
  }
  .icon {
    .youtube {
      margin-right: 30px;
    }
    .twitter {
      margin-right: 30px;
    }
    .facebook {
      margin-right: 30px;
      margin-top: 6px;
    }
    .google {
      margin-right: 30px;
      margin-top: 7px;
    }
  }
  h2 {
    font-family: "Work Sans", sans-serif;
    padding-top: 10px;
    font-weight: 400;
    font-size: 20px;
    color: #96839b;
  }
}

@media (max-width: 1380px) {
  .seti{
    h4{
      font-size: 18px;
      padding-bottom: 22px;
    }
    h2{
      padding-bottom: 22px;

    }
  }
}
</style>
