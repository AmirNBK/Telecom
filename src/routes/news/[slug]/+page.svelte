<script>
    import "../../../app.css";
    import Footer from "../../../components/Footer/Footer.svelte";
    import Header from "../../../components/Header/Header.svelte";
    import HeroSection from "../../../components/HeroSection/HeroSection.svelte";
    import Product from "../../../components/Products/Product.svelte";
    import SideBar from "../../../components/SideBar/SideBar.svelte";
    import Tags from "../../../components/Tags/Tags.svelte";
    import product1 from "../../../assets/image/product1.jpeg";
    import ContactUs from "../../../components/ContactUs/ContactUs.svelte";
    import ItemSwitcher from "../../../components/ItemSwitcher/ItemSwitcher.svelte";
    import logo from "../../../assets/icons/logo.svg";
    import HeadlineComponent from "../../../components/HeadlineComponent/HeadlineComponent.svelte";
    import News from "../../../components/News/News.svelte";
    import NewsItems from "../../../components/News/NewsItems/NewsItems.svelte";
    import SingleNews from "../../../components/SingleNews/SingleNews.svelte";
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
    <a href="/">
        <img
            src={logo}
            alt="logo"
            class="mx-auto mt-8 block sm:hidden w-28 md:w-52 rounded-md"
            style="background-color: #9C1511;"
        />
    </a>
    <HeroSection />
    <div class="flex lg:flex-row flex-col gap-10 mx-auto" style="width: 90%;">
        <div class="flex flex-col" style="flex : 1">
            <SideBar />
            <Tags />
        </div>
        <div style="flex : 2.5;">
            <div class="">
                <div class="mb-6 flex flex-col gap-6">
                    <div
                        class="ContactUsContainer rounded-md pb-8"
                        style="box-shadow: 0px 4px 80px 0px rgba(0, 0, 0, 0.10);"
                    >
                        <h2
                            style="background-color: #0E3552;"
                            class="text-xl rounded-t-md text-white px-4 py-2"
                        >
                            News
                        </h2>
                        <SingleNews
                            title="Optical Transceiver Interoperability and compatibility Guida"
                            date="Friday, October 14, 2022"
                            description="what Does SFP Compatibility Mean? & Main Concerns for Buying Compatible Optical Transceiver what Does SFP Compatibility Mean? & Main Concerns for Buying Compatible Optical Transceiver what Does SFP Compatibility Mean? & Main Concerns for Buying Compatible Optical Transceiver what Does SFP Compatibility Mean? & Main Concerns for Buying Compatible Optical Transceiver"
                        />
                    </div>
                </div>
            </div>
        </div>
    </div>

    <Footer />
</div>
