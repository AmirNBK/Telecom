<script lang="ts">
    export let title : string;
    export let date : string;
    export let description : string;
</script>

<div class="NewsItemContainer flex flex-col gap-10 pb-4 p-6">
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
</div>
