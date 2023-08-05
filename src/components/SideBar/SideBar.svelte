<script>
    import SideBarItems from "./SideBarItems/SideBarItems.svelte";


</script>


<div class="SideBar w-3/12 text-white bg-white ml-16 mb-12 rounded-md" style="box-shadow: 0px 0px 16px -5px #000000;">
    <div class="SideBar__title text-xl mb-2 px-2 py-4 rounded-t-md" style="background : #0E3552">
        Categories
    </div>
    <div class="SideBar__items flex flex-col gap-1 pb-2">
        <SideBarItems name='Digital voice switching'/>
        <SideBarItems name='Security'/>
        <SideBarItems name='5G'/>
        <SideBarItems name='Data Routing'/>
        <SideBarItems name='Digital PBX'/>
    </div>
</div>