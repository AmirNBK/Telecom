<script>
    import image from "../../assets/image/product1.jpeg";
    import Modal from "../Modal/Modal.svelte";

    let showModal = false;
</script>

<div>
    <div
        class="ProductsContainer rounded-md pb-8"
        style="box-shadow: 0px 4px 80px 0px rgba(0, 0, 0, 0.10);"
    >
        <h2
            style="background-color: #0E3552;"
            class="text-xl rounded-t-md text-white px-4 py-2"
        >
            product
        </h2>
        <img src={image} alt="image" class="mx-auto rounded-md mt-4 w-6/12" />

        <div class="flex flex-col justify-center gap-6 items-center mt-6">
            <h2 class="text-2xl text-center font-medium">GS100</h2>
            <p class="text-sm sm:text-xl text-center">
                huaweiBBU3900BBU3910GM5DOGTMUC00_Main Control and Transportuni
                NEW
            </p>

            <p class="price font-medium text-xl" style="color: #DC0600;">
                $400.00 excl tax
            </p>
            <button
                on:click={() => (showModal = true)}
                class="rounded-md py-2 px-6 w-fit text-sm mt-2 text-white"
                style="background-color: #9C1511;">Add to cart</button
            >
        </div>
        <Modal bind:showModal>
            <h2 slot="header">Please enter your information</h2>

            <ol class="definition-list">
                <li class="text-center mt-4">
                    <input
                        class="w-6/12 py-2 px-4 rounded-md"
                        style="border: 1px solid gray;"
                        placeholder="enter your name"
                    />
                </li>
                <li class="text-center mt-4">
                    <input
                        class="w-6/12 py-2 px-4 rounded-md"
                        style="border: 1px solid gray;"
                        placeholder="enter your email"
                    />
                </li>

                <li class="text-center mt-4">
                    <button
                        class="rounded-md py-2 px-6 w-fit text-sm mt-2 text-white"
                        style="background-color: #9C1511;">Add to cart</button
                    >
                </li>
            </ol>
        </Modal>

        <div class="ml-4 mt-3 md:p-0 pr-4" />
    </div>
</div>
