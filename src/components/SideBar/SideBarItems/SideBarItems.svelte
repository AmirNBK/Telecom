<script>
    export let name;
    import play from '../../../assets/icons/play.svg'
</script>

<div class="SideBarItems rounded-md mx-2 py-2 px-4 flex flex-row items-center gap-3" style="background : #0E3552">
    <img src={play} class="w-3" alt="play"/>
    <p class="w-fit text-xl"> {name} </p>
</div>