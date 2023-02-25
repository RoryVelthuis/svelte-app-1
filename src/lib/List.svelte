<script>
    export let items = [];

    export let value = '';
    export function AddItem(){
        items = [...items, value]
        console.log(items);
    }
</script>

<style>
    h3{
        margin: 0;
    }
    .list{
        margin: 0px 5px;
    }
</style>

<div class="list">
    <h3>List</h3>
    <input bind:value={value}>
    <button on:click={() => AddItem()}>Add</button>
    <ul>
        {#each items as item, index}
            <li>
                {item}
            </li>
        {/each}
    </ul>
</div>