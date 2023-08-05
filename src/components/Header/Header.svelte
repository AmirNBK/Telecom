<script>
    const headerItems = [
        "Register",
        "Login",
        "Shopping cart(0)",
        "compare product list",
        "wishlist",
        "Us dollar",
        "English",
    ];
</script>

<div
    class="Header flex flex-row justify-center gap-10 py-4"
    style="box-shadow:rgb(0, 0, 0) 0px 0px 10px -5px"
>
    {#each headerItems as items, index}
        <div>
            {items}
        </div>
    {/each}
</div>
