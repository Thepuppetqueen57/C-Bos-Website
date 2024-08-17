<script lang="ts">
  import Buttons from "./lib/Buttons.svelte";
</script>
  
<main>
  <div class="container">
    <h1>C-Bos</h1>
    <Buttons />
  </div>
</main>
  
<style lang="scss">
  $purple: #370664;
  $purpletext: #420068;
  $lightgray: #b6b6b6;

  :global(body), :global(html) {
    overflow: hidden;
    height: 100%;
    margin: 0;
  }
  
  main {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Arial, sans-serif;
  }
  
  .container {
    text-align: center;
  }
  
  h1 {
    margin-bottom: 20px;
    color: $purpletext;
  }
</style>