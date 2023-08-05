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
</script>

<div style="background-color: #9C1511;" class="text-white py-4 flex justify-center gap-10">
    {#each items as items, index}
        <div>
            {items}
        </div>
    {/each}
</div>
