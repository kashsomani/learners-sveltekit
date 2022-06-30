<script>
    import Carousel from "./_components/carousel.svelte";
</script>

<div id="main">
    <div class="hero min-h-screen">
        <div class="hero-content text-center">
            <div class="max-w-md">
                <div class="grid grid-cols-1 place-items-center">
                    <img src="/assets/old_logo.png" alt="logo" width="50%" />
                </div>
                <h1 class="text-5xl font-bold text-primary">
                    Learners' Academy
                </h1>
                <p class="py-6 text-justify">
                    Learners’ Academy was established in June 1983 with only
                    Pre-Primary and Primary sections. Today, we have classes up
                    to Std. X (I.C.S.E.). We have grown with our children to
                    give our community a home where learning begins and from
                    where emerge the citizens of tomorrow. We have cutting-edge
                    technologies coupled with experienced teachers to cater to
                    the intrinsic as well as extrinsic devlopments of all
                    children. With STEM being our primary focus, our alumni have
                    consistently gone forward to work in various industries such
                    as medicine, engineering, technology and many more
                </p>
                <!-- maybe add something like this in future -->
                <!-- <button class="btn btn-primary">Get Started</button> -->
            </div>
        </div>
    </div>

    <Carousel />
</div>

<style lang="postcss">
    #main {
        @apply bg-lime-100;
    }
</style>
