<script lang="ts">
    function redirect(url: string) {
        window.location.href = url
    }

    const infourl = "https://thepuppet57.alwaysdata.net/tps/cbos/info.html"
    const packagelisturl = "https://thepuppet57.alwaysdata.net/tps/cbos/packagelist"
    const repourl = "https://github.com/Thepuppetqueen57/C-Bos"
    const backendurl = "https://thepuppet57.alwaysdata.net/tps/cbos/backend"
</script>

<main>
    <div class="button-container">
        <button on:click={(event) => redirect(infourl)}>Info</button>
        <button on:click={(event) => redirect(packagelisturl)}>Package List</button>
        <button on:click={(event) => redirect(repourl)}>Source Code</button>
        <button on:click={(event) => redirect(backendurl)}>Backend</button>
    </div>
</main>

<style lang="scss">
  $purple: #370664;
  $purpletext: #420068;
  $lightgray: #b6b6b6;

  .button-container {
    display: flex;
    gap: 5px;
  }

  button {
    background-color: $purple;
    color: $lightgray;
    width: 90px;
    height: 40px;
    border-radius: 10px;
    border: none;
    transition: 0.3s;
  }

  button:hover {
    transform: scale(1.1);
    background-color: darken($purple, 3);
  }
</style>