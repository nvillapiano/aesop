<template>
  <div class="wrapper">
    <Sidenav />
    <main class="main-content">
      <hr class="ae-mar-0">
      <hr class="ae-mar-0">
      <hr class="ae-mar-0">
      <hr class="ae-mar-0">
      <!-- Loop through component data to populate docs -->
      <Doc
        :title="componentData.title"
        :id="componentData.title.toLowerCase().split(' ').join('_')"
        :description="componentData.description"
        :color="componentData.color"
        :example="componentData.example"
        :code="componentData.code"
      />
    </main>

  </div>
</template>

<script>
// import Sidenav from '@/components/sidenav.vue'
import Doc from '@/components/Doc.vue'
import Sidenav from '@/components/Sidenav.vue'
import { componentData } from '../components/component-docs'

export default {
  name: 'Home',
  components: {
    Doc,
    Sidenav
  },
  data () {
    return {
      componentData: componentData
    }
  }
}
</script>

<style lang="scss">
  .color-blocks,
  .text-blocks {
    display: flex;
  }

  .color-blocks {
    display: flex;
    align-items: center;
    justify-content: center;

    div {
      box-shadow: 0px 2px 8px rgba(18,22,25,0.5);
      width: 5rem;
      height: 5rem;
      margin: 1rem;

      &:first-of-type {
        margin-left: 0;
      }
    }
  }

  .button-with-input {
    display: flex;
    align-items: center;
  }

  .input-styles {

    input {
      display: block;
    }
  }

  section[id*="Code"] {

    .description + hr,
    .example,
    .example + hr {
      display: none;
    }
  }
</style>
