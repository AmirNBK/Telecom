<script>
    const items = [
        "ALCATEL",
        "CISCO",
        "JUNIPER",
        "MARCONI",
        "NEWBRIDGE",
        "NOKIA",
        "NORTEL",
        "OTHER PRODUCTS",
    ];
    import home from "../../assets/icons/home.svg";
</script>

<div
    style="background-color: #9C1511;"
    class="text-white py-5 flex justify-center items-center"
>
    <img src={home} alt="home" class="w-7 absolute left-12" />
    <div class="flex justify-center gap-10">
        {#each items as items, index}
            <div>
                {items}
            </div>
        {/each}
    </div>
</div>
