<script>
    import Step from "./Step.svelte";

    let steps = [
        { name: "Project 1", icon: "fa-solid fa-cart-shopping" },
        { name: "Project 2", icon: "fa-solid fa-list-check" },
        { name: "Project 3", icon: "fa-solid fa-diagram-project" },
    ];

    let benefits = [
        {
            name: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
            description:
                "Etiam posuere porttitor fermentum. Sed varius vitae odio a dictum. Donec fringilla erat urna, et sollicitudin ex pulvinar sed. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Morbi finibus ultricies sem, eget feugiat enim consectetur ac",
        },
        {
            name: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
            description:
                "Etiam posuere porttitor fermentum. Sed varius vitae odio a dictum. Donec fringilla erat urna, et sollicitudin ex pulvinar sed. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Morbi finibus ultricies sem, eget feugiat enim consectetur ac",
        },
        {
            name: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
            description:
                "Etiam posuere porttitor fermentum. Sed varius vitae odio a dictum. Donec fringilla erat urna, et sollicitudin ex pulvinar sed. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Morbi finibus ultricies sem, eget feugiat enim consectetur ac",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-1ß"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">Maheem</span>
                Pome <br />Full Stack
                <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:lext-lg md:text-xl">
                My <span class="text-violet-400">favorite tech</span> include JavaScript
                (Angular or SvelteKit), Tailwind CSS, Node.js + Express.js & GraphQL
                or Firebase/Firestore!
            </p>
            <a
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer"
                href="linkedin.com"
                target="_blank"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                ></div>
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile.png"}
                alt="profile_image"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
    </section>

    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        <a
            href="https://www.youtube.com"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play"></i>
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-col-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit.<strong
                        class="text-violet-400"
                        >Sed do eiusmod tempor incididunt ut labore et dolore
                        magna aliqua.</strong
                    >Ut enim ad minim veniam, quis nostrud exercitation ullamco
                    laboris nisi ut aliquip ex ea commodo consequat.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit.<strong
                        class="text-violet-400"
                        >Sed do eiusmod tempor incididunt ut labore et dolore
                        magna aliqua.</strong
                    >Ut enim ad minim veniam, quis nostrud exercitation ullamco
                    laboris nisi ut aliquip ex ea commodo consequat.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit.<strong
                        class="text-violet-400"
                        >Sed do eiusmod tempor incididunt ut labore et dolore
                        magna aliqua.</strong
                    >Ut enim ad minim veniam, quis nostrud exercitation ullamco
                    laboris nisi ut aliquip ex ea commodo consequat.
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
            <h3 class="font-semibold text-xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        <h5 class="text-2xl sm:text-3xl font-semibold text-center poppins">
            The <span class="text-violet-400 poppins">Complete</span> Package
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class="border-b border-solid border-slate-200">
                    <tr>
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th
                            class="whitespace-nowrap bg-violet-700 text-white p-4 px-8"
                            >Me</th
                        >
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
                            >Dedication</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-check text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-check text-green-500"></i></td
                        >
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
                            >Critical Thought</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-check text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-check text-green-500"></i></td
                        >
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
                            >Interpersonal Skills</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-check text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-check text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-check text-green-500"></i></td
                        >
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
                            >Programming Ability</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-check text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td
                        >
                        <td><i class="fa-solid fa-check text-green-500"></i></td
                        >
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not invest?</p>
    </section>
</main>
