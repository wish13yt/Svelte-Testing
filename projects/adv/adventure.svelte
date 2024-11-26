<style>
    * {
        color: white;
    }
    button {
        background-color: black;
    }
</style>
<script>
    let fate = ""
    function path1() {
        fate = "You enjoy making websites more!"
    }
    function path2() {
        fate = "You still enjoy making sites, just a little less."
    }
</script>
<h1>Svelte Adventure!</h1>
<button on:click={path1}>Svelte</button>
<button on:click={path2}>Plain HTML</button>
<h2>Your Fate</h2>
<p>{fate}</p>