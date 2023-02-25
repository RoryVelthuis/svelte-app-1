<script>
        export let title = "Svelte App";

        export const pages = [
            {
                title: "Home",
                link: "/"
            },
            {
                title: "About",
                link: "/about"
            }
        ];
</script>

<style>
    .nav-bar{
        display: flex;
        align-items: center;
        width: 100%;
        height: 50px;
        margin: 0;
        padding: 0;
        background-color: lightblue;
    }

    .nav-bar nav{
        display: flex;
        align-items: center;
        height: 100%;
    }

    h1{
        font-size: 20px;
        padding: 0px 10px
    }

    .nav-list{
        list-style: none;
        display: flex;
        align-items: center;
        height: 100%;
        padding: 0;
        margin: 0;
    }
    .nav-list li{
        display: flex;
        align-items: center;
        padding: 0px 10px;
        height: 100%;
    }
    .nav-list li:hover{
        background-color: rgb(160, 206, 221);
    }
</style>

<div class="nav-bar">
    <h1>{title}</h1>
    <nav>
        <ul class="nav-list">
            {#each pages as page, i}
            <li><a href="{page.link}">{page.title}</a></li>
            {/each}

        </ul>
    </nav>
</div>