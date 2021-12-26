<template>
  <div class="boilerplate" :class="`ae-bg-${color}`">
    <h1>Aēsop UI</h1>
    <h4 :class="`ae-invert`">A minimal CSS framework inspired by the skin care brand <a href="http://www.aesop.com">Aēsop</a>.</h4>
    <p style="max-width: 500px;">Example text with <a href="#">Link style</a>. Lorem ipsum dolor, sit amet consectetur adipisicing elit. Amet tenetur tempora similique. Officiis fugiat ea dolorum veritatis iure aliquam, reprehenderit magnam autem, excepturi dolor necessitatibus aperiam nesciunt quae corrupti doloribus?</p>
    <button class="ae-button">Button</button> <button class="ae-button ae-secondary">Secondary</button>
    <br>
    <form>
      <input type="text" placeholder="Input"><button class="ae-button">Button</button>
    </form>
    <form action="">
      <textarea name="" id="" cols="30" rows="10" placeholder="Textarea">Message...</textarea>
    </form>
    <ul>
      <li>List item 1</li>
      <li>List item 2</li>
      <li>List item 3</li>
      <li>List item 4</li>
    </ul>
    <ol>
      <li>List item 1</li>
      <li>List item 2</li>
      <li>List item 3</li>
      <li>List item 4</li>
    </ol>
    <ul class="ae-list-unstyled">
      <li>List item 1</li>
      <li>List item 2</li>
      <li>List item 3</li>
      <li>List item 4</li>
    </ul>
    <code class="ae-code-block">
      <pre>&lt;script&gt;
  export default {
    name: 'Boilerplate',
    props: {
      color: String
    }
  }
&lt;/script&gt;</pre>
    </code>
    <span class="ae-code-inline ae-display-inline-block ae-mar-b-1">ae-code-inline</span>
    <table style="max-width: 600px;" class="ae-table">
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
    </table>

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

  form {
    display: flex;
    align-items: center;
  }
</style>
