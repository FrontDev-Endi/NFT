<template>
  <div class="input">
    <input type="email" id="email" placeholder="info@gmail.com" />
    <button type="submit" id="submit">Subscribe</button>
  </div>
</template>

<style lang="scss" scoped>
.input {
  display: flex;
  justify-content: center;
  margin-top: 25px;
  padding-bottom: 117px;
  input {
    width: 436px;
    height: 96px;
    padding-left: 53px;
    border: #e7b226 1px solid;
    font-family: "Work Sans", sans-serif;
    font-weight: 400;
    font-size: 24px;
    color: #a48ea9;
  }
  button {
    font-family: "Work Sans", sans-serif;
    // width: 244px;
    // height: 96px;
    padding: 30px 64px;
    background: #e7b226;
    font-weight: 700;
    font-size: 24px;
    color: #251928;
  }
}
@media (max-width: 1380px) {
  .input {
    input {
      width: 336px;
      height: 86px;
    }
    button{
      font-size: 23px;
    }
  }
}

@media (max-width: 768px) {
  .input {
    input {
      width: 236px;
      height: 86px;
      padding-left: 27px;
      font-size: 18px;
    }
    button{
      font-size: 18px;
      padding: 20px 54px;
    }
  }
}

@media (max-width: 600px) {
  .input {
    input {
      width: 206px;
      height: 66px;
      padding-left: 27px;
      font-size: 18px;
    }
    button{
      font-size: 16px;
      padding: 20px 34px;
    }
  }
}
</style>
