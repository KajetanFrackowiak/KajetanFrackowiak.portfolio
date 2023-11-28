<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "Deep Learning Specialization",
            icon: "fa-solid fa-brain",
            description:
                "A package of projects created following Andrew Ng's advice, related to deep learning with Tensorflow.",
            githubLink:
                "https://github.com/KajetanFrackowiak/DeepLearningSpecialization",
        },
        {
            name: "Machine Learning Specialization",
            icon: "fa-solid fa-robot",
            description:
                "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
            githubLink: "https://github.com/KajetanFrackowiak/freeCodeCamp",
        },
        {
            name: "Properties of Compact Groups of Galaxies",
            icon: "fa-solid fa-network-wired",
            description:"Delve into astrophysics with the project, unraveling the dynamics and behaviors of densely packed galaxy collections.",
            githubLink:
                "https://github.com/KajetanFrackowiak/PropertiesofCompactGroupsofGalaxies",
        },
    ];

    
    let benefits = [
        {
            name: "Data Science Explorer",
            icon: "fas fa-chart-bar",
            description:
                "I enjoy tinkering with data, crafting algorithms, and unraveling hidden patterns to make sense of the numbers. It's like solving puzzles, but with data!",
        },
        {
            name: "Machine Learning Tinkerer",
            icon: "fas fa-robot",
            description:
                "I'm all about playing with Machine Learning, making things learn and adapt. Think of it like teaching computers some cool tricks! It's a bit like magic, but with more code.",
        },
        {
            name: "Deep Learning Adventurer",
            icon: "fas fa-globe",
            description:
                "In the vast universe of Deep Learning, I'm on a quest to design, train, and optimize neural networks using cool tools like OpenCV, Pandas, Numpy, Scipy, and Matplotlib. It's a bit like training a digital brain to do awesome things!",
        },
        {
            name: "Python Enthusiast",
            icon: "fab fa-python",
            description:
                "My go-to language is Python. It's like the Swiss Army knife for coding - handy, versatile, and perfect for all sorts of adventures! Python helps me bring my ideas to life in the digital world.",
        },
        {
            name: "Linux Enthusiast",
            icon: "fab fa-linux",
            description:
                "I'm passionate about Linux. Exploring its open-source ecosystem, customizing my workspace, and embracing the power of the command line are some of my favorite Linux adventures. The penguin (Tux) is my coding companion!",
        },
        {
            name: "Communication and Interests",
            icon: "fas fa-comments",
            description:
                "Beyond coding, I value effective communication in a professional setting. I believe in the power of clear, concise, and friendly communication. Whether it's collaborating on a project, presenting ideas, or explaining complex concepts, I strive to foster a positive and collaborative environment in any work setting. Let's connect and share ideas!",
        },
        {
            name: "Additional Interests",
            icon: "fas fa-chess",
            description:
                "Outside of work, you might find me strategizing on a chessboard or exploring the mysteries of the cosmos. I have a keen interest in languages, and I'm always eager to learn something new!",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">Kajetan</span>
                Frąckowiak
                <br /> Passionate about
                <span class="poppins text-violet-400">Deep Learning</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400"> favorite tech</span> includes Python
                (Tensorflow, Keras, Pytorch, Scikit-learn, Pandas, Linux) or Weight
                & Biases!
            </p>
            <button
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
                onclick="redirectGitHub()"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                ></div>
                <h4 class="relative z-9">GIT &rarr;</h4>
            </button>

            <script>
                function redirectGitHub() {
                    window.location.href =
                        "https://github.com/KajetanFrackowiak";
                }
            </script>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile.png"}
                alt="Zetane Engine"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
        <!-- <div  class="flex p-0.5 relative max-w-[700px] w-full mx-auto">
            <div
                class="absolute inset-0 overflow-hidden rounded-md flex items-center justify-center"
            >
                <div
                    class="bg-gradient-to-r absolute inset-[-20px]  from-violet-800 to-indigo-800 specialSpin"
                />
            </div>

            <img
                src={"images/zetane-engine.jpeg"}
                alt="Zetane Engine"
                class="w-full h-full object-cover z-[2]"
            />
        </div> -->
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

        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    Embark on a journey through the realm of deep learning with
                    a curated package of projects inspired by <strong>
                        Andrew Ng's
                    </strong>
                    teachings, unraveling the intricacies of neural networks and
                    their applications
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Explored various aspects of machine learning in FreeCodeCamp
                    projects, including cost regression, text classification for
                    spam detection, and a book recommendation system.
                </p>
            </Step>

            <Step step={steps[2]}>
                <p>
                    Dive into astrophysics with this project on Compact Groups
                    of Galaxies (CGs). Use Python's statistical methods to
                    explore galaxy merging and interactions. No prior knowledge
                    needed — join for an enriching experience!
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <!-- <div class="flex flex-col gap-2 mx-auto">
                    <div class="flex items-end gap-4">
                        <p
                            class="poppins text-6xl sm:text-7xl md:text-8xl text-slate-500 font-medium"
                        >
                            {benefit.metric}
                        </p>
                        <p
                            class="text-xl sm:text-2xl md:text-3xl capitalize pb-2"
                        >
                            {benefit.name}
                        </p>
                    </div>
                    <p class="text-center italic">- {benefit.description}</p>
                </div> -->
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
        <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
            The <span class="text-violet-400">Complete</span> Package
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class={"border-b border-solid border-slate-200  "}>
                    <tr class="">
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th
                            class="bg-violet-700 text-white whitespace-nowrap p-4 px-8"
                            >Me</th
                        >
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Dedication</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Critical Thought</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr>
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Interpersonal Skills</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Progamming Ability</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
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
