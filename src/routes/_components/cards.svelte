<script>
    import { cardData } from "./card-data";
    import { images } from "./carousel-data";
</script>

<div class="grid grid-cols-2 place-items-center px-6 gap-4">
    {#each cardData as card}
        <div class="card card-side bg-lime-200 shadow-xl">
            <figure>
                <img src={card.src} alt={images.alt} class="h-full" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">{card.alt}</h2>
                <p>{card.descr}</p>
                <div class="card-actions justify-end">
                    <button class="btn btn-neutral w-16"
                        ><img src="./assets/email.png" alt="Movie" /></button
                    >
                </div>
            </div>
        </div>
    {/each}
</div>
