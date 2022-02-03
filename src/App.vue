<template>
  <router-view/>
</template>

<style lang="scss">
  @import "./scss/index.scss";

  #app {
    overflow: hidden;
    overflow-y: initial;
  }

  .wrapper {
    display: flex;

    .main-content {
      width: 100%;
    }
  }
</style>
