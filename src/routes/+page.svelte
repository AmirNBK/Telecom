<script>
    import "../app.css";
    import Footer from "../components/Footer/Footer.svelte";
    import Header from "../components/Header/Header.svelte";
    import HeroSection from "../components/HeroSection/HeroSection.svelte";
    import Product from "../components/Product/Product.svelte";
    import SideBar from "../components/SideBar/SideBar.svelte";
    import Tags from "../components/Tags/Tags.svelte";
    import product1 from "../assets/image/product1.jpeg";
</script>

<div>
    <Header />
    <HeroSection />
    <div class="flex flex-col ml-20">
        <SideBar />
        <Tags />
    </div>
    <Product
        brand="Microwava"
        name="03031 MXR"
        description="huaweiBBU3900BBU3910GM5DOGTMUC00_Main Control and Transportuni NEW"
        price="$400.00"
        image={product1}
    />
    <Footer />
</div>
