<script setup>
import Item from "./Item-list.vue";
import Arrow from "./Arrow.vue";
</script>
<template>
  <div class="list">
    <Item
      Icon="/src/assets/img/wallet.svg"
      Text="Set up your wallet"
      Alt="wallet"
    />
    <Arrow />
    <Item
      Icon="/src/assets/img/liberi.svg"
      Text="Create your collection"
      Alt="liberi"
    />
    <Arrow />
    <Item Icon="/src/assets/img/add.svg" Text="Add your NFTs" Alt="Add" />
    <Arrow />
    <Item
      Icon="/src/assets/img/statik.svg"
      Text="Create your collection"
      Alt="liberi"
    />
  </div>
</template>

<style lang="scss" scoped>
.list {
  display: flex;
  justify-content: center;
}
@media (max-width: 1390px) {
  .list {
    margin-left: 0px;
  }
}
@media (max-width: 1100px) {
  .list {
    flex-direction: column;
    margin-top: -100px;
  }
}
</style>
