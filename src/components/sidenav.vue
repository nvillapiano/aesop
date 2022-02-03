<template>

  <nav class="side-nav ae-bg-black">
    <ul class="ae-list-unstyled">
      <li class="ae-heading-4" v-for="component in componentData" :key="component.title">
        <!-- <router-link class="ae-link-unstyled" :to="'#' + `${component.title.toLowerCase().split(' ').join('_')}`">{{component.title}}</router-link> -->
        <router-link class="ae-link-unstyled" :to="{path: component.title}">{{component.title}}</router-link>
      </li>
    </ul>
  </nav>

</template>

<script>
import { componentData } from '../components/component-docs'

export default {
  name: 'Sidenav',
  data () {
    return {
      componentData: componentData
    }
  },
  mounted() {
    const el = document.querySelector(this.$route.hash)
    el && el.scrollIntoView()

    console.log(el)
  }
}
</script>

<style lang="scss">
  @import "../scss/_variables.scss";

  .side-nav {
    position: fixed;
    top: 0;
    left: 0;
    height: 100vh;
    padding: 3rem 0.5rem;
    border-right: 3px solid $black;
    width: 250px;

    & + * {
      margin-left: 250px;
    }

    li {

      a {
        padding: 0 0.5rem;
      }
    }
  }
</style>
