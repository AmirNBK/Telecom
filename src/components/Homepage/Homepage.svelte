<script>
    import image from "../../assets/image/homepagePic.png";
    import FeaturedProducts from "../FeaturedProducts/FeaturedProducts.svelte";
    import HeadlineComponent from "../HeadlineComponent/HeadlineComponent.svelte";
    import imageProduct from "../../assets/image/featuredProduct1.jpeg";
    import News from "../News/News.svelte";

    const featuredProducts = [
        {
            name: "03054886",
            description:
                "huaweiBBU3900BBU3910GM5DOGTMUC00_Main Control and Transportuni NEW",
            image: imageProduct,
        },
        {
            name: "03054886",
            description:
                "huaweiBBU3900BBU3910GM5DOGTMUC00_Main Control and Transportuni NEW",
            image: imageProduct,
        },
        {
            name: "03054886",
            description:
                "huaweiBBU3900BBU3910GM5DOGTMUC00_Main Control and Transportuni NEW",
            image: imageProduct,
        },
    ];
</script>

<div>
    <div
        class="HomePaggContainer rounded-md pb-4"
        style="box-shadow: 0px 4px 80px 0px rgba(0, 0, 0, 0.10);"
    >
        <h2
            style="background-color: #0E3552;"
            class="text-xl rounded-t-md text-white px-4 py-2"
        >
            Welcome to our store
        </h2>
        <img src={image} alt="image" class="rounded-md mt-4 w-11/12 mx-auto" />
    </div>

    <div class="my-6">
        <HeadlineComponent title="Featured products" />
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-8 mt-6">
            {#each featuredProducts as product}
                <FeaturedProducts
                    name={product.name}
                    description={product.description}
                    image={product.image}
                />
            {/each}
        </div>
    </div>

    <div class="my-6 flex flex-col gap-6">
        <HeadlineComponent title="News" />
        <News />
    </div>
</div>
