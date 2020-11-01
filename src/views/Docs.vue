<template>
  <div class="wrapper">
    <!-- <Sidenav /> -->
    <main class="main-content">
      <hr class="ae-mar-0">
      <hr class="ae-mar-0">
      <hr class="ae-mar-0">
      <hr class="ae-mar-0">
      <!-- Typography -->
      <Doc
        title="Typography"
        description='
          The Aēsop official website uses the font <a href="https://www.swisstypefaces.com/fonts/suisse/">Suisse</a>.
          Aēsop CSS uses a close analog, <a href="https://fonts.google.com/specimen/DM+Sans">DM Sans</a>.
          The six heading classes are provided along with a general body font.
          Also included is the utility class <span class="ae-code-inline">ae-invert</span>, a class that adds a black background and pseudo-knockout text,
          and <span class="ae-code-inline">ae-code-inline</span>, a class for displaying pieces of code inline.
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
<p class="ae-invert ae-mar-b-2" style="max-width: 800px;">
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio corrupti,
  placeat consequuntur explicabo culpa cupiditate laborum vero sint deleniti
  esse iure adipisci aut atque perspiciatis sequi tempora facere cumque vitae!
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio corrupti,
  placeat consequuntur explicabo culpa cupiditate laborum vero sint deleniti
  esse iure adipisci aut atque perspiciatis sequi tempora facere cumque vitae!
</p>
<span class="ae-code-inline">ae-code-inline</span>'
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
      <!-- Color -->
      <Doc
        title="Color"
        description="The colors in Aēsop are based on the colors of the various packages, tubes, jars, etc. used by the Aēsop brand. These colors were grabbed via eyedropper from images of the packages themselves, capturing the tone as accurately as possible. Colors are meant to be used in large blocks, applied to backgrounds only, using the invert class for needed contrast."
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
      <!-- Buttons -->
      <Doc
        title="Buttons"
        description="Buttons in Aēsop CSS are meant to be simple and minimalistic, with only two variations: Standard and Secondary. There are no size options tied to buttons, but buttons tied to inputs will shrink to match the size of the input."
        color="tan"
        example='
<!-- Button styles -->
<div class="button-styles">
  <button>Standard</button>
  <button class="ae-secondary">Secondary</button>
</div>

<!-- Classes can be used to apply button styles to non-button elements -->
<div class="button-application">
  <a href="#" class="ae-button">Standard</a>
  <a href="#" class="ae-button ae-secondary">Secondary</a>
</div>

<!-- Buttons tied to inputs receive the input size -->
<div class="button-with-input">
  <input type="text" placeholder="Input"><button class="ae-button">Button</button>
</div>'
      />
      <!-- Inputs -->
      <Doc
        title="Inputs"
        color="blue"
        example='
<div class="input-styles">
  <!-- Text -->
  <input type="text" placeholder="Input">

  <!-- Date -->
  <input type="date" placeholder="">

  <!-- Time -->
  <input type="time" placeholder="">

  <!-- Password -->
  <input type="password" placeholder="">

  <!-- Textarea -->
  <textarea placeholder="Textarea"></textarea>
</div>

<!-- Buttons tied to inputs receive the input size -->
<div class="button-with-input">
  <input type="text" placeholder="Input"><button class="ae-button">Button</button>
</div>'
      />
      <!-- Lists -->
      <Doc
        title="Lists"
        color="pink"
        example='
<div class="list-styles">

  <!-- Unordered -->
  <ul class="ae-list-unordered ae-mar-b-2">
    <li>
      List item 1
    </li>
    <li>
      List item 2
    </li>
    <li>
      List item 3
    </li>
    <li>
      List item 4
    </li>
  </ul>

  <!-- Ordered -->
  <ol class="ae-list-ordered ae-mar-b-2">
    <li>
      List item 1
    </li>
    <li>
      List item 2
    </li>
    <li>
      List item 3
    </li>
    <li>
      List item 4
    </li>
  </ol>

  <!-- Unstyled -->
  <ul class="ae-list-unstyled ae-mar-b-2">
    <li>
      List item 1
    </li>
    <li>
      List item 2
    </li>
    <li>
      List item 3
    </li>
    <li>
      List item 4
    </li>
  </ul>
</div>'
      />
      <!-- Code blocks -->
      <Doc
        title="Code blocks"
        color="grey"
        example='
  <!-- Code block example -->
  <code class="ae-code-block">
    <pre>
      ...
    </pre>
  </code>'
      />
      <!-- Tables -->
      <Doc
        title="Tables"
        color="orange"
        example='
<table class="ae-table">
  <thead>
    <tr>
      <th>Column 1</th>
      <th>Column 2</th>
      <th>Column 3</th>
      <th>Column 4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Data 1.1</td>
      <td>Data 2.1</td>
      <td>Data 3.1</td>
      <td>Data 4.1</td>
    </tr>
    <tr>
      <td>Data 1.2</td>
      <td>Data 2.2</td>
      <td>Data 3.2</td>
      <td>Data 4.2</td>
    </tr>
    <tr>
      <td>Data 1.3</td>
      <td>Data 2.3</td>
      <td>Data 3.3</td>
      <td>Data 4.3</td>
    </tr>
    <tr>
      <td>Data 1.4</td>
      <td>Data 2.4</td>
      <td>Data 3.4</td>
      <td>Data 4.4</td>
    </tr>
  </tbody>
</table>'
      />
      <!-- Checkboxes -->
      <Doc
        title="Checkboxes"
        color="green"
        example='
<form class="ae-checkbox-container">
  <input type="checkbox" id="ae_checkbox_example_1" class="ae-checkbox" value="option1" />
  <label for="ae_checkbox_example_1">Option 1</label>
  <input type="checkbox" id="ae_checkbox_example_2" class="ae-checkbox" value="option1" />
  <label for="ae_checkbox_example_2">Option 1</label>
  <input type="checkbox" id="ae_checkbox_example_3" class="ae-checkbox" value="option1" />
  <label for="ae_checkbox_example_3">Option 1</label>
</form>
'
      />
      <!-- Radio buttons -->
      <Doc
        title="Radio buttons"
        color="tan"
        example='
<form class="ae-radio-container" role="group">
  <input type="radio" id="ae_radio_example_1" class="ae-radio" value="option1" name="ae-radio-example" />
  <label for="ae_radio_example_1">Option 1</label>
  <input type="radio" id="ae_radio_example_2" class="ae-radio" value="option1" name="ae-radio-example" />
  <label for="ae_radio_example_2">Option 1</label>
  <input type="radio" id="ae_radio_example_3" class="ae-radio" value="option1" name="ae-radio-example" />
  <label for="ae_radio_example_3">Option 1</label>
</form>
'
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
