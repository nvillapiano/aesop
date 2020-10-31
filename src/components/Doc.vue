<template>

  <section class="doc" :id="title" :class="`ae-bg-${color}`">
    <h1 class="title ae-mar-t-5 ae-mar-b-2">{{title}}</h1>
    <h2 class="description ae-heading-5 ae-invert ae-pad-1 ae-pad-r-4 ae-mar-b-1" v-html="description"></h2>
    <hr class="ae-mar-t-b-5">
    <div v-html="example" class="example"></div>
    <hr class="ae-mar-t-b-5">
    <code class="ae-code-block">
      <pre v-if="code">
        {{code}}
      </pre>
      <pre v-else>
        {{example}}
      </pre>
    </code>
    <hr class="ae-mar-t-5 ae-mar-b-0">
    <hr class="ae-mar-0">
    <hr class="ae-mar-0">
    <hr class="ae-mar-0">
  </section>

</template>

<script>
export default {
  name: 'Sidenav',
  props: {
    title: String,
    description: String,
    color: String,
    example: String,
    code: String
  }
}
</script>

<style lang="scss">
  @import "../scss/_variables.scss";

  .doc {
    padding: 0 2rem 0;
    min-height: 100vh;
    overflow: hidden;

    .description {
      // max-width: 800px;
      // width: 100%;
    }

    code {
      padding-top: 0;
      padding-bottom: 0;
    }
  }

</style>
