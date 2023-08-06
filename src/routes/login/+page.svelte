<script>
    import "../../app.css";
    import Footer from "../../components/Footer/Footer.svelte";
    import Header from "../../components/Header/Header.svelte";
    import HeroSection from "../../components/HeroSection/HeroSection.svelte";
    import Product from "../../components/Product/Product.svelte";
    import SideBar from "../../components/SideBar/SideBar.svelte";
    import Tags from "../../components/Tags/Tags.svelte";
    import product1 from "../../assets/image/product1.jpeg";
    import ContactUs from "../../components/ContactUs/ContactUs.svelte";
    import ItemSwitcher from "../../components/ItemSwitcher/ItemSwitcher.svelte";
    const products = [
        {
            brand: "Microwava",
            name: "03031 MXR",
            description:
                "huaweiBBU3900BBU3910GM5DOGTMUC00_Main Control and Transportuni NEW",
            price: "$400.00",
            image: product1,
        },
        {
            brand: "TechX",
            name: "TX5000",
            description:
                "Advanced Wireless Router with High-Speed Connectivity",
            price: "$250.00",
            image: product1,
        },
        {
            brand: "GigaStream",
            name: "GS100",
            description:
                "Smart Streaming Device for High-Quality Entertainment",
            price: "$99.99",
            image: product1,
        },
        {
            brand: "EcoCharge",
            name: "ECO-2000",
            description: "Fast-Charging Power Bank with Long Battery Life",
            price: "$49.99",
            image: product1,
        },
        {
            brand: "SmartFit",
            name: "SF-500",
            description: "Fitness Tracker with Heart Rate Monitor and GPS",
            price: "$129.00",
            image: product1,
        },
        {
            brand: "SmartFit",
            name: "SF-500",
            description: "Fitness Tracker with Heart Rate Monitor and GPS",
            price: "$129.00",
            image: product1,
        },
    ];
</script>

<div>
    <Header />
    <HeroSection />
    <div class="flex flex-row gap-10 mx-auto" style="width: 90%;">
        <div class="flex flex-col" style="flex : 1">
            <SideBar />
            <Tags />
        </div>
        <div style="flex : 2.5;">
            
            <div class="mt-14">
                <ItemSwitcher items={["New products", "LTE"]} />
                <div class="grid grid-cols-3 gap-8 mt-6">
                    {#each products as product}
                        <Product
                            brand={product.brand}
                            name={product.name}
                            description={product.description}
                            price={product.price}
                            image={product.image}
                        />
                    {/each}
                </div>
            </div>
        </div>
    </div>

    <Footer />
</div>
