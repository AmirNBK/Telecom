<script>
    const headerItems = [
        "Shopping cart(0)",
        "compare product list",
        "wishlist",
        "Us dollar",
        "English",
    ];
</script>

<div
    class="Header flex flex-row justify-center gap-10 py-4 flex-wrap"
    style="box-shadow:rgb(0, 0, 0) 0px 0px 10px -5px"
>
    {#each headerItems as item, index}
        {#if item === "Login" || item === "Register"}
            <a href="/login" class="cursor-pointer">
                {item}
            </a>
        {:else}
            <div>
                {item}
            </div>
        {/if}
    {/each}
</div>
