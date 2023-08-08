<script lang="ts">
    export let title: string;
    export let date: string;
    export let description: string;
</script>

<div
    class="NewsItemContainer flex flex-col gap-10 pb-4"
    style="border-bottom: 1px solid gray;"
>
    <div
        class="NewsItemContainer__headline flex justify-between"
        style="color : #DC0600"
    >
        <p class="text-xs sm:text-base">{title}</p>
        <p class="text-xs sm:text-base">{date}</p>
    </div>
    <div class="font-medium text-sm sm:text-base">
        {description}
    </div>
    <a href="/news/items">
        <div class="text-end">
            <button
                class="rounded-md py-2 px-6 w-fit text-sm mt-2 text-white"
                style="background-color: #9C1511;">details</button
            >
        </div>
    </a>
</div>
