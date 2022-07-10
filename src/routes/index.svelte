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
    <div class="grid grid-cols-1 place-items-center">
        <p class="py-6 mx-28 text-justify">
            Learners’ Academy, established in 1983, has strived since its
            conception to mould the children of today into extraordinary and
            responsible individuals of tomorrow. Learners’ has always
            prioritized the total growth of a child’s character and personality.
            Curiosity and competence with compassion is encouraged, hence, life
            is learning at Learners’. Affiliated to the Council For The Indian
            School Certificate Examinations (I.C.S.E examination at class X
            level), Learners’ is a progressive co-educational institution which
            aims at an application based learning experience. The school employs
            a well-qualified, trained and experienced teaching staff and an
            excellent support staff that ensures the all-round development of
            the students. The school’s counselling department caters to students
            with learning difficulties and ensures inclusive education. With
            extensive use of diversified methodologies and teaching expertise,
            we are committed to the mission of helping each child realize her or
            his maximum potential. Learners’ offers a variety of extracurricular
            activities to help students meet their full potential. Students
            participate in sessions of Speech and drama, Western Dance, Music
            and instruments which help them to deepen their social and
            intellectual growth. Intra house debates, drama, elocutions,
            singing, essay writing competitions are periodically held to nurture
            a healthy competitive spirit in our students. In addition, sports
            and games activities like swimming, football, carrom, volleyball
            ensure the physical and mental wellbeing of our students. The school
            has a well-equipped infrastructure with a library, a science
            laboratory, computer laboratory, activity room and a dedicated STEM
            department to cater to the educational needs of students.
            Interactive displays and smart boards in every class helps the
            teacher simplify concepts with the help of technology. As one of the
            oldest and best rated educational institutions at Bandra, Learners’
            stays committed to its goal of providing a holistic educational
            environment to its students.
        </p>
    </div>
</div>

<style lang="postcss">
    #main {
        @apply bg-lime-100;
    }
</style>
