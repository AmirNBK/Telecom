<script>
    const headerItems = [
        { text: "Home", url: "/" },
        { text: "Products", url: "/products" },
        { text: "Contact us", url: "/contact-us" },
        { text: "About us", url: "/about-us" },
        { text: "English", url: "#" },
    ];
</script>

<div
    class="Header flex flex-row justify-center gap-10 py-4 flex-wrap"
    style="box-shadow:rgb(0, 0, 0) 0px 0px 10px -5px"
>
    {#each headerItems as item, index}
        {#if item.text === "Login" || item.text === "Register"}
            <a href={item.url} class="cursor-pointer">
                {item.text}
            </a>
        {:else}
            <a href={item.url} class="cursor-pointer">
                {item.text}
            </a>
        {/if}
    {/each}
</div>
