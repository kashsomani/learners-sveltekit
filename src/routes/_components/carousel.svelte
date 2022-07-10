<script>
    import { images } from "./carousel-data";
    import { goto } from "$app/navigation";

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
                                id="slide-{image.id}"
                                class="carousel-item relative w-full"
                            >
                                <img src={image.src} class="w-full" />
                                <div
                                    class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
                                >
                                    <a
                                        href="#slide-{image.id - 1 >= 0
                                            ? image.id - 1
                                            : images.length - 1}"
                                        class="btn btn-circle">❮</a
                                    >
                                    <a
                                        href="#slide-{image.id + 1 <
                                        images.length
                                            ? image.id + 1
                                            : 0}"
                                        class="btn btn-circle">❯</a
                                    >
                                </div>
                            </div>
                        {/each}
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
