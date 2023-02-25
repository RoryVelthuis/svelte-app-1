<script>
    export let title = "Svelte App";
    console.log(title);

    export let count = 0;
</script>

<h1>Welcome to {title}</h1>

<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<button on:click={() => count++}>Click</button>
<p>{count}</p>