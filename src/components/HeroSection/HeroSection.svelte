<script>
    import Navigation from "../Navigation/Navigation.svelte";
    import SearchInput from "../SearchInput/SearchInput.svelte";
</script>

<div
    class="mx-auto my-12 flex flex-col justify-between"
    style="background-color: blueviolet; width: 90%;height: 500px"
>
    <div class="flex flex-row justify-end pt-6 mr-6">
        <SearchInput placeholder="Search store" />
        <button
            style="background-color: #9C1511;"
            class="text-white rounded-md py-1 px-4"
        >
            Search
        </button>
    </div>

    <div>
        <Navigation />
    </div>
</div>
