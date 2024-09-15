<script setup>
import Cart from "./Cart-colle.vue";

import { ref } from "vue";

const blocknot = ref(false);
const btnnot = ref(true);

const open = () => {
  blocknot.value = true;
  btnnot.value = false;
};
</script>

<template>
  <div class="collection">
    <div class="one">
      <div class="one-block wow animate__animated animate__fadeInLeft">
        <Cart imageUrl="/src/assets/img/ava.svg" />
        <Cart imageUrl="/src/assets/img/ava 3.svg" />
      </div>
      <div class="two-block wow animate__animated animate__fadeInRight">
        <Cart imageUrl="/src/assets/img/ava 2.svg" />
        <Cart imageUrl="/src/assets/img/ava 4.svg" />
      </div>
    </div>
    <div class="two" v-if="blocknot">
      <div class="one-block">
        <Cart imageUrl="/src/assets/img/ava.svg" />
        <Cart imageUrl="/src/assets/img/ava 3.svg" />
      </div>
      <div class="two-block">
        <Cart imageUrl="/src/assets/img/ava 2.svg" />
        <Cart imageUrl="/src/assets/img/ava 4.svg" />
      </div>
    </div>
    <div v-if="btnnot" class="btn-all" @click="open">
      <button>View All</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.collection {
  .one {
    display: flex;
    justify-content: center;
    margin-top: 80px;
    .one-block {
      margin-right: 72px;
    }
  }
  .two {
    display: flex;
    justify-content: center;
    .one-block {
      margin-right: 72px;
    }
  }
  .btn-all {
    display: flex;
    justify-content: center;
    padding-bottom: 80px;
    button {
      font-family: "Work Sans", sans-serif;
      justify-content: center;
      background: transparent;
      margin-top: 28px;
      border: 1px solid #ffce4e;
      // width: 257px;
      // height: 84px;
      padding: 24px 64px;
      font-weight: 500;
      font-size: 30px;
      line-height: 1.18174;
      letter-spacing: 0.05em;
      color: #f5fbf2;
      transition: all 0.2s ease;
    }
    @media (hover: hover) {
      button:hover {
        box-shadow: inset 0 -3.25em 0 0 var(--gold-five);
      }
    }
    @media (hover: none) {
      button:active {
        box-shadow: inset 0 -3.25em 0 0 var(--gold-five);
      }
    }
  }
}
@media (max-width: 1380px) {
  .collection {
    .btn-all {
      button {
        font-size: 25px;
      }
    }
  }
}

@media (max-width: 1100px) {
  .collection {
    .one {
      flex-direction: column;
      align-items: center;
      .one-block {
        margin-right: 0;
      }
    }
    .two {
      flex-direction: column;
      align-items: center;
      .one-block {
        margin-right: 0;
      }
    }
  }
}
</style>
