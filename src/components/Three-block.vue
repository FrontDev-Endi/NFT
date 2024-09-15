<script setup></script>

<template>
  <div>
    <div class="about">
      <h1>Support</h1>
      <div class="list">
        <p>Help & Support</p>
        <p>Item Details</p>
        <p>Author Profile</p>
        <p>Collection</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.about {
  margin-top: 50px;
  margin-left: 227px;
  h1 {
    font-family: "Work Sans", sans-serif;
    padding-bottom: 18px;
    font-weight: 700;
    font-size: 24px;
    color: #f5fbf2;
  }
  .list {
    p {
      font-family: "Work Sans", sans-serif;
      cursor: pointer;
      font-weight: 500;
      font-size: 20px;
      line-height: 2.525;
      color: #96839b;
    }
  }
}
@media (max-width: 1380px) {
  .about {
    margin-left: 78px;
  }
}

@media (max-width: 1100px) {
  .about {
    .list {
      p {
        font-size: 16px;
      }
    }
  }
}
</style>
