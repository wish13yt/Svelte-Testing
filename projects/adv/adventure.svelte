<style>
    * {
        color: white;
    }
    button {
        background-color: black;
    }
</style>
<script>
    let fate1 = ""
    let fate2 = ""
    let svelte = ""
    let html = ""
    function path1() {
        fate1 = "You enjoy making websites more!"
        svelte = true
    }
    function path2() {
        fate1 = "You still enjoy making sites, just a little less."
        html = true
    }
    function path3() {
        if (svelte == true) {
            fate2 = "Your house explodes"
        } else {
            fate2 = "You used the correct thing! Your program works and deploys successfully!"
        }
    }
    function path4() {
        if (html == true) {
            fate2 = "Your house explodes"
        } else {
            fate2 = "You used the correct thing! Your program works and deploys successfully!"
        }
    }
</script>
<h1>Svelte Adventure!</h1>
<h2>Round 1</h2>
<button on:click={path1}>Svelte</button>
<button on:click={path2}>Plain HTML</button>
<h2>Your Fate (Round 1)</h2>
<p>{fate1}</p>
<h2>Round 2</h2>
<button on:click={path3}>onclick=</button>
<button on:click={path4}>on:click=</button>
<h2>Your Fate (Round 2)</h2>
<p>{fate2}</p>