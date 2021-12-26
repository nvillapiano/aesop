<template>
  <div class="wrapper">
    <!-- <Sidenav /> -->
    <main class="main-content">
      <Doc
        title="Typography"
        description='
          The Aēsop official website uses the font <a href="https://www.swisstypefaces.com/fonts/suisse/">Suisse</a>.
          Aēsop UI uses a close analog, <a href="https://fonts.google.com/specimen/DM+Sans">DM Sans</a>.
          The six heading classes are provided along with a general body font.
          Also included is the utility class <a href="#">ae-invert</a>, a class that adds a black background and pseudo-knockout text.
        '
        color="orange"
        example='
<!-- Heading classes -->
<div class="ae-mar-b-2">
  <h1 class="ae-display-inline ae-mar-r-2">
    Heading 1
  </h1>
  <h2 class="ae-display-inline ae-invert ae-pad-l-r-2">
    ae-heading-1
  </h2>
</div>
<div class="ae-mar-b-2">
  <h2 class="ae-display-inline ae-mar-r-2">
    Heading 2
  </h2>
  <h3 class="ae-display-inline ae-invert ae-pad-l-r-2">
    ae-heading-2
  </h3>
</div>
<div class="ae-mar-b-2">
  <h3 class="ae-display-inline ae-mar-r-2">
    Heading 3
  </h3>
  <h4 class="ae-display-inline ae-invert ae-pad-l-r-1">
    ae-heading-3
  </h4>
</div>
<div class="ae-mar-b-2">
  <h4 class="ae-display-inline ae-mar-r-2">
    Heading 4
  </h4>
  <h5 class="ae-display-inline ae-invert ae-pad-l-r-1">
    ae-heading-4
  </h5>
</div>
<div class="ae-mar-b-2">
  <h5 class="ae-display-inline ae-mar-r-2">
    Heading 5
  </h5>
  <h6 class="ae-display-inline ae-invert">
    ae-heading-5
  </h6>
</div>
<div class="ae-mar-b-2">
  <h6 class="ae-display-inline ae-mar-r-2">
    Heading 6
  </h6>
  <h6 class="ae-display-inline ae-invert">
    ae-heading-6
  </h6>
</div>
<p style="max-width: 800px;">
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio corrupti,
  placeat consequuntur explicabo culpa cupiditate laborum vero sint deleniti
  esse iure adipisci aut atque perspiciatis sequi tempora facere cumque vitae!
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio corrupti,
  placeat consequuntur explicabo culpa cupiditate laborum vero sint deleniti
  esse iure adipisci aut atque perspiciatis sequi tempora facere cumque vitae!
</p>
<p class="ae-invert" style="max-width: 800px;">
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio corrupti,
  placeat consequuntur explicabo culpa cupiditate laborum vero sint deleniti
  esse iure adipisci aut atque perspiciatis sequi tempora facere cumque vitae!
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio corrupti,
  placeat consequuntur explicabo culpa cupiditate laborum vero sint deleniti
  esse iure adipisci aut atque perspiciatis sequi tempora facere cumque vitae!
</p>'
        code='
<!-- Styles applied to HTML -->
<h1>
  ...
</h1>

<!-- Styles applied to via class -->
<div class="ae-heading-1">
  ...
</div>

<!-- Classes override HTML styles -->
<h1 class="ae-heading-6">
  ...
</h1>

<!-- Invert -->
<h1 class="ae-invert">
  ...
</h1>'

      />
      <Doc
        title="Color"
        description="The colors in Aēsop are based on the colors of the various packages, tubes, jars, etc. used by the Aēsop brand."
        color="green"
        example='
<!-- Background classes -->

<div class="color-blocks">
  <div class="ae-bg-orange"></div>
  <div class="ae-bg-green"></div>
  <div class="ae-bg-tan"></div>
  <div class="ae-bg-blue"></div>
  <div class="ae-bg-pink"></div>
  <div class="ae-bg-grey"></div>
  <div class="ae-bg-black"></div>
  <div class="ae-bg-white"></div>
</div>'

      />
    </main>

  </div>
</template>

<script>
// import Sidenav from '@/components/sidenav.vue'
import Doc from '@/components/Doc.vue'

export default {
  name: 'Home',
  components: {
    // Sidenav,
    Doc
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

</style>
