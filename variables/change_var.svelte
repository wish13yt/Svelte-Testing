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
    function func2() {
        testVar = "Hello"
    }
</script>
<h1>{testVar}</h1>
<button on:click={func}>change to "world!"</button>
<button on:click={func2}>revert</button>