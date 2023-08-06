<script>
    export let name;
    export let description;
    export let image;
</script>

<style>
    .Product {
        border: 1px solid #0E3552;
        width: 250px;
        height: 380px;
        justify-content: space-between;
    }

    .Product h2 {
        margin: 0;
    }

    .Product img {
        height: auto;
        border-radius: 0.25rem;
        box-shadow: 0px 4px 25px 0px rgba(0, 0, 0, 0.50);
    }

    .Product .description {
        text-align: center;
        font-size: 0.875rem;
        max-width: 100%;
        overflow-wrap: break-word;
    }

    .Product .price {
        color: #DC0600;
        font-weight: 500;
        margin: 0;
    }

    .Product button {
        background-color: #9C1511;
        color: white;
        border: none;
        padding: 0.4rem 1.2rem;
        cursor: pointer;
    }
</style>

<div class="Product flex flex-col w-fit rounded-2xl pt-3 justifty-between mx-auto">
    <div class="flex flex-col items-center gap-y-2">
        <img class="rounded-md rounded-2xl w-52" src={image} alt="product" />
        <h2 class="">{name}</h2>
        <div class="description px-4 mt-6">{description}</div>
    </div>

    <div class="flex flex-col items-center">
        <button class="rounded-b-2xl py-3 px-6 w-full text-sm mt-2 text-lg" style="text-decoration : underline">Request Only</button>
    </div>
</div>
