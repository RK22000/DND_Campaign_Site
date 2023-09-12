<script>
    import CharacerBar from "./CharacerBar.svelte";
    import Bjorn from "./Bjorn.svelte";
</script>

<CharacerBar color_class='bg-persian_red' title='Umbral Ranger' image_src='/pics/umbral_ranger.png'>
    <p class="flex items-center justify-center w-full h-full">
        Umbral Ranger is a mysterious stranger
    </p>
</CharacerBar>

<CharacerBar color_class='bg-peach' title='Bjorn Ironoak' image_src='/pics/bjorn_ironoak.jpg'>
    <div>
        <Bjorn/>
    </div>
</CharacerBar>

<CharacerBar color_class='bg-aero'/>
