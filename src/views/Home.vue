<template>
  <div class="home">
    <main class="main-content">
      <Boilerplate color="orange"/>
      <Boilerplate color="blue"/>
      <Boilerplate color="pink"/>
      <Boilerplate color="green"/>
      <Boilerplate color="grey"/>
      <Boilerplate color="tan"/>
    </main>

  </div>
</template>

<script>
import Boilerplate from '@/components/boilerplate.vue'

export default {
  name: 'Home',
  components: {
    Boilerplate
  }
}
</script>

<style lang="scss">

  .home {
    display: flex;

    .main-content {
      width: 100%;
    }
  }

</style>
