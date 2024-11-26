<style>
    * {
        color: white;
    }
    button {
        background-color: black;
    }
</style>
<script>
    let testVar = "Hello"
    function func() {
        testVar = "World!"
    }
</script>
<h1>{testVar}</h1>
<button on:click={func}>h</button>