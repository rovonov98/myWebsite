<template>
    <div class="burger">
      <div class="burger-layer"></div>
      <div class="burger-layer"></div>
      <div class="burger-layer"></div>
    </div>
</template>

<style scoped lang="scss">
.burger {
      cursor: pointer;
      position: fixed;
      z-index: 3;       
      max-width: 100%; 
      top: 2vh;
      left: 3vw;
      right: 0;
      padding: 2em;
    }
  .burger-layer {
      width: 20px;
      height: 2px;
      background-color: $main-color-one;
      margin: 3px;
  }
</style>