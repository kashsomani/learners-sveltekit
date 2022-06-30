<script>
    import { images } from "./carousel-data";
    import { goto } from "$app/navigation";

    function routeToPage(route, replaceState) {
        goto(`/${route}`, { replaceState });
    }
    let currentIndex = 0;
</script>

<div class="grid grid-cols-1 place-items-center w-full">
    <div class="grid grid-cols-1 place-items-center w-full">
        <div class="card w-9/12 bg-lime-50 text-primary-content">
            <div class="card-body pt-6">
                <div class="grid grid-cols-1 place-items-center">
                    <div class="carousel w-full">
                        {#each images as image}
                            <div
                                id="slidshow-image-{image.id}"
                                class="carousel-item w-full grid grid-cols-1 place-items-center"
                            >
                                <img src={image.src} class="w-3/4 rounded-lg" />
                            </div>
                        {/each}
                    </div>
                    <div class="flex justify-center w-full py-2 ">
                        <div class="btn-group">
                            {#each images as image}
                                <a
                                    class="btn btn-lg {currentIndex === image.id
                                        ? 'btn-active'
                                        : ''}"
                                    href="#slidshow-image-{image.id}"
                                    on:click={() => (currentIndex = image.id)}
                                    >{image.id + 1}</a
                                >
                            {/each}
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
