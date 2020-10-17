<template>
  <div class="home">
    <Boilerplate color="orange"/>
    <Boilerplate color="blue"/>
    <Boilerplate color="pink"/>
    <Boilerplate color="green"/>
    <Boilerplate color="grey"/>
    <Boilerplate color="tan"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Boilerplate from '@/components/boilerplate.vue'

export default {
  name: 'Home',
  components: {
    Boilerplate
  }
}
</script>

<style lang="scss">

  .card {
    padding: 2rem;
  }

</style>
