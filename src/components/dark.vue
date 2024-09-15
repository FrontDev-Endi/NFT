<template>
  <div class="dark">
    <h1 class="btn">Place a Bid</h1>
  </div>
</template>

<style lang="scss" scoped>
.dark {
  position: absolute;
  margin-top: -306px;
  width: 351px;
  height: 306px;
  background: rgba(0, 0, 0, 0.65);
  z-index: 10;
  .btn {
    font-family: "Work Sans", sans-serif;
    margin-top: 118px;
    margin-left: auto;
    margin-right: auto;
    width: 72%;
    padding: 21px 57px;
    backdrop-filter: blur(45px);
    background: #ffce4e;
    font-weight: 600;
    font-size: 24px;
    color: #000;
    cursor: pointer;
  }
}
.hidden {
  display: none;
}

@media (max-width: 500px) {
  .dark {
    width: 241px;
    height: 241px;
    margin-top: -241px;
    .btn {
      font-size: 19px;
      padding: 21px 33px 21px 33px;
      margin-top: 90px;
    }
  }
}
</style>
