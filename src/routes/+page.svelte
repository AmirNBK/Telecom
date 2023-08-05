<script>
    import "../app.css";
    import Header from "../components/Header/Header.svelte";
    import HeroSection from "../components/HeroSection/HeroSection.svelte";
    import SideBar from "../components/SideBar/SideBar.svelte";
    import Tags from "../components/Tags/Tags.svelte";
</script>

<div>
    <Header />
    <HeroSection />
    <div class="flex flex-col">
        <SideBar />
        <Tags />
    </div>
</div>
