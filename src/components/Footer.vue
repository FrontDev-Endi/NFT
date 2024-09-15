<script setup>
import One from "./One-block.vue";
import Two from "./Two-block.vue";
import Three from "./Three-block.vue";
</script>

<template>
  <div id="footer">
    <div id="logo">
      <img src="../assets/img/logo.png" alt="logo" />
    </div>
    <div class="xer">
      <One />
      <div class="xyu">
        <Two />
        <Three />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#footer {
  width: 100%;
  height: 100%;
  justify-content: center;
  background: #251928;
  display: flex;
  #logo {
    width: 194px;
    height: 194px;
    margin-top: 50px;
    img{
      width: 194px;
      height: 194px;  
    }
  }
  .xyu {
    display: flex;
  }

  .xer {
    display: flex;
  }
}

@media (max-width: 1000px) {
  #footer {
    flex-direction: column;
    #logo {
      margin-left: auto;
      margin-right: auto;
    }
    .xer{
      display: flex;
      justify-content: center;
    }
  }
}

@media (max-width: 768px) {
  #footer {
    .xer{
      margin-left: auto;
      margin-right: auto;
      flex-direction: column;
      .seti{
        h4{
          font-size: 20px;
        }
      }
    }
  }
}
</style>
