<script>
    import {base} from '$app/paths'
    export let color_class = 'bg-persian_red';
    $: text_color = ['bg-persian_red', 'bg-aero', 'bg-bg-davys_gray'].includes(color_class) ? 'text-misty_rose' : 'text-davys_gray';
    export let image_src=`${base}/pics/PaperDragons.jpg`;
    export let title="Title";
    
</script>

<div class='{color_class} font-sans'>
        <h1 class="text-center pb-5 {text_color}">{title}</h1>
    <div class="pb-5">
        <div class='bg-davys_gray/90 flex'>
            <div class="w-1/2 aspect-[2/1] overflow-hidden rounded-xl">
                <div class="w-full h-full bg-cover bg-center transition hover:scale-125 brightness-75 hover:brightness-100 duration-1000" style="background-image: url({image_src});"/>
            </div>
            <div class="w-1/2 text-misty_rose">
                <slot >
                    <p class="w-full h-full flex justify-center items-center">
                        Sphinx of black quartz judge my vow.
                    </p>
                </slot>
            </div>
            <!-- <p class="w-1/2 flex items-center justify-center text-misty_rose">{content}</p> -->
        </div>
    </div>
</div>