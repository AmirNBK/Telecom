<script>
    export let text;
    export let icon;
</script>

<div class="relative w-6/12 pb-2" style="border-bottom : 2px solid #2B7EB0">
    <img src={icon} class="w-5 absolute left-0" style="transform: translateY(2px);" />
    <input placeholder={text} class="outline-none pl-7" />
</div>
