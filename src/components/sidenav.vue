<template>

  <nav class="side-nav ae-bg-black">
    <ul class="ae-list-unstyled">
      <li class="ae-heading-4">
        <a class="ae-link-unstyled" href="#">Typography</a>
      </li>
      <li class="ae-heading-4">
        <a class="ae-link-unstyled" href="#">Color</a>
      </li>
      <li class="ae-heading-4">
        <a class="ae-link-unstyled" href="#">Colors</a>
      </li>
      <li class="ae-heading-4">
        <a class="ae-link-unstyled" href="#">Buttons</a>
      </li>
      <li class="ae-heading-4">
        <a class="ae-link-unstyled" href="#">Inputs</a>
      </li>
      <li class="ae-heading-4">
        <a class="ae-link-unstyled" href="#">Lists</a>
      </li>
      <li class="ae-heading-4">
        <a class="ae-link-unstyled" href="#">Code blocks</a>
      </li>
      <li class="ae-heading-4">
        <a class="ae-link-unstyled" href="#">Tables</a>
      </li>
    </ul>
  </nav>

</template>

<script>
export default {
  name: 'Sidenav'
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
