<script>
    import { images } from "./carousel-data";
</script>

<div class="grid grid-cols-1 place-items-center w-full">
    <div class="grid grid-cols-1 place-items-center w-1/2">
        <div class="carousel w-full">
            {#each images as image}
                <div
                    id="slidshow-image-{image.id}"
                    class="carousel-item w-full"
                >
                    <img src={image.src} class="w-full" />
                </div>
            {/each}
        </div>
        <div class="flex justify-center w-full py-2 gap-2">
            {#each images as image}
                <a href="#slidshow-image-{image.id}" class="btn btn-xs"
                    >{image.id + 1}</a
                >
            {/each}
        </div>
    </div>
</div>
