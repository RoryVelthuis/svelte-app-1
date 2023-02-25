<script>
    export let count = 0;
</script>

<style>
    .counter{
        margin: 10px 5px;
    }
    h3{
        margin: 0;
    }
    p{
        margin: 0px 10px;

    }
    .controls{
        display: flex;
    }
</style>

<div class="counter">
    <h3>Counter</h3>
    <div class="controls">
        <button on:click={() => count++}>Click</button>
        <p>{count}</p>
    </div>
</div>