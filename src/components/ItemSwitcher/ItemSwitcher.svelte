<script>
    export let items;
</script>

<div class="items-baseline flex flex-row gap-2 pl-4" style="border-bottom: 1px solid #000;">
    {#each items as items}
        <div
            style="background: rgba(218, 218, 218, 0.25); border: 1px solid rgba(0, 0, 0, 0.10);"
            class="rounded-t-md py-2 px-4 cursor-pointer"
        >
            {items}
        </div>
    {/each}
</div>
