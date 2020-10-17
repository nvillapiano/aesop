<template>
  <div class="boilerplate" :class="`ae-bg-${color}`">
    <h1>Hello world!</h1>
    <h4 :class="`ae-invert-${color}`">Lorem ipsum dolor sit amet consectetur adipisicing elit.</h4>
    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Amet tenetur tempora similique. Officiis fugiat ea dolorum veritatis iure aliquam, reprehenderit magnam autem, excepturi dolor necessitatibus aperiam nesciunt quae corrupti doloribus?</p>
    <button class="ae-button">Button</button> <button class="ae-button ae-secondary">Secondary</button> <button class="ae-button ae-tertiary">Tertiary</button>
  </div>
</template>

<script>
export default {
  name: 'Boilerplate',
  props: {
    color: String
  }
}
</script>

<style scoped lang="scss">
  .boilerplate {
    padding: 2rem;
  }
</style>
