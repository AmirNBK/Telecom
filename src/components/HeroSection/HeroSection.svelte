<script>
    import Navigation from "../Navigation/Navigation.svelte";
    import SearchInput from "../SearchInput/SearchInput.svelte";
    import HeroSectionImage from "../../assets/image/HeroSectionImage.png";
    import logo from '../../assets/icons/logo.svg'
</script>

<div
    class="mx-auto my-12 flex flex-col justify-between relative"
    style="width: 90%;height: 500px;"
>
    <img src={HeroSectionImage} alt="image" class="w-full absolute" style="height: 500px;" />
    <img src={logo} alt="logo" class="absolute w-52"/>
    <div class="flex flex-row justify-end pt-6 mr-6 absolute right-0">
        <SearchInput placeholder="Search store" />
        <button
            style="background-color: #9C1511;"
            class="text-white rounded-md py-1 px-4"
        >
            Search
        </button>
    </div>

    <div class="absolute bottom-0 w-full">
        <Navigation />
    </div>
</div>
