<template>
  <div class="wrapper">
    <main class="main-content">
      <hr class="ae-mar-0">
      <hr class="ae-mar-0">
      <hr class="ae-mar-0">
      <hr class="ae-mar-0">
      <!-- Loop through component data to populate docs -->
      <Doc v-for="component in componentData" :key="component.title"
        :title="component.title"
        :description="component.description"
        :example="component.example"
        :code="component.code"
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
  <input type="radio" id="ae_radio_example_2" class="ae-radio" value="option2" name="ae-radio-example" />
  <label for="ae_radio_example_2">Option 2</label>
  <input type="radio" id="ae_radio_example_3" class="ae-radio" value="option3" name="ae-radio-example" />
  <label for="ae_radio_example_3">Option 3</label>
</form>
'
      />
      <!-- Block quotes -->
      <Doc
        title="Block quotes"
        color="grey"
        example='
<blockquote class="ae-blockquote">
  <q class="ae-quote">
    Decay is inherent upon all compounded things; strive on with diligence.
  </q>
  <cite class="ae-cite">Siddhartha Gautama</cite>
</blockquote>
'
      />
      <!-- Select menus -->
      <Doc
        title="Select menus"
        color="orange"
        example='
<form>
  <label for="select-menu-example" class="ae-label">Select one:</label>
  <select class="ae-select" id="select-menu-example" required>
    <option value="1">Option 1</option>
    <option value="2">Option 2</option>
    <option value="3">Option 3</option>
  </select>
</form>
        '
      />
    </main>

  </div>
</template>

<script>
// import Sidenav from '@/components/sidenav.vue'
import Doc from '@/components/Doc.vue'
import { componentData } from '../components/component-docs'

export default {
  name: 'Home',
  data () {
    return {
      componentData: componentData
    }
  },
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

  section.doc {
    background: var(--ae-orange);
  }
</style>
