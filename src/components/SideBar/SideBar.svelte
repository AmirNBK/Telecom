<script lang="ts">
    import { createEventDispatcher } from "svelte";
    import SideBarItems from "./SideBarItems/SideBarItems.svelte";

    const dispatch = createEventDispatcher();

    let selectedCategory: string | null = null;

    const categoryNames = [
        "Digital voice switching",
        "Security",
        "Add and Drop Multiplexer",
        "5G",
        "Data Routing",
        "Digital PBX",
    ];

    const products = ["TX3000", "TX3000", "GS5100", "UBC23RE"];

    function toggleCategory(category: string) {
        if (selectedCategory === category) {
            selectedCategory = null;
        } else {
            selectedCategory = category;
        }
        dispatch("categoryToggle", selectedCategory);
    }
</script>

<div
    class="SideBar w-full text-white bg-white mb-8 rounded-md"
    style="box-shadow: 0px 0px 16px -5px #000000;"
>
    <div
        class="SideBar__title text-xl mb-2 px-2 py-4 rounded-t-md"
        style="background : #0E3552"
    >
        Categories
    </div>
    <div class="SideBar__items flex flex-col gap-1 pb-2">
        {#each categoryNames as categoryName}
            <div
                class="cursor-pointer"
                on:click={() => toggleCategory(categoryName)}
            >
                <SideBarItems name={categoryName} />
            </div>
            {#if selectedCategory === categoryName}
                <div class="ml-4 text-sm text-gray-500 my-4">
                    <p class="text-xl text-center text-black">
                        {categoryName} products
                    </p>
                    <ul class="flex flex-col gap-2 mt-2 text-lg">
                        {#each products as items}
                            <li
                                style="border-bottom: 1px solid #eee;"
                                class="w-11/12"
                            >
                                {items}
                            </li>
                        {/each}
                    </ul>
                </div>
            {/if}
        {/each}
    </div>
</div>
