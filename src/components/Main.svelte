<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "BI",
            icon: "fa-solid fa-cart-shopping",
            description:
                "The Global Electronics Store Analytics is a BI project using Tableau, analyzing e-commerce data with KPIs, Excel, and OLAP tools. It provides actionable insights into sales, customer behavior, and performance metrics to drive business decisions",
        },
        {
            name: "Machine Learning",
            icon: "fa-solid fa-list-check",
            description:
                "The Customer Satisfaction Predictor is a Python-based machine learning project that predicts customer satisfaction by analyzing relevant features. With data-driven insights, it helps improve customer experience and satisfaction levels. Analyze and optimize!",
        },
        {
            name: "WEB programming",
            icon: "fa-solid fa-diagram-project",
            description:
                "The Personal Workout Planner is a Next.js & TailwindCSS web application, built with Node.js, that generates personalized workout plans based on user-defined goals and areas to improve. Get stronger, faster, and fitter!",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "Aspiring Data & Business Analyst",
            description:
                "I am passionate about turning data into insights that drive better decisions and business improvements. With hands-on experience in data analysis and process optimization, I enjoy using data to understand trends, identify opportunities, and solve complex business challenges. I'm always learning new tools and methodologies to better analyze data and deliver impactful solutions.",
        },
        {
            name: "Strong Communicator & Collaborative Team Player",
            description:
                "Clear communication and collaboration are essential to me. I believe in leveraging the strengths of diverse teams, and I’m committed to transparency and constructive dialogue. My interpersonal skills help me work effectively with team members, ensuring a productive and positive working environment.",
        },
        {
                name: "a self taught developer",
            description:
                "I taught myself to code using free online resources and absolutely fell in love with the creativity and problem solving that is involved in developing and engineering innovative new online experiences. Starting of with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, design, cloud services and much much more.",
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
            <h2 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Hi! I'm <span class="poppins bg-gradient-to-r text-transparent text-transparent font-bold bg-gradient-to-r from-pink-500 to-violet-400 bg-clip-text">Shahar</span> Levi Atias
                <br />Industrial Engineering 
                <span class="poppins text-transparent text- font-bold bg-gradient-to-r from-pink-500 to-violet-400 bg-clip-text">& Management</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-300"> expertise lies </span> in data analysis, process optimization, and strategic planning. I’m passionate about transforming data into actionable insights and streamlining processes to drive impactful results.
                <br>In addition, I know how to program with JavaScript
                (NEXT.JS and SvelteKit), TailwindCSS, Node.js.</p>
            <button
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <a href="#footer" class="relative z-9">
                    <h4>Get in touch</h4>
                </a>
            </button>
        </div>
        <div class="relative shadow-1xl grid place-items-center">
            <img
                src={"images/profile.webp"}
                alt="shahar image AI"
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
        <a
            href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    The Global Electronics Store Analytics is a <strong
                    class="text-violet-400"
                    >BI </strong> project using Tableau, analyzing e-commerce data with <strong
                        class="text-violet-400">KPIs, Excel,</strong> and  <strong
                        class="text-violet-400">OLAP </strong> tools.
                         It provides actionable insights into sales, customer behavior, and performance metrics to drive business decisions.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    The Customer Satisfaction Predictor is a <strong class="text-violet-400"
                    >Python</strong>
                -based 
                <strong class="text-violet-400">machine learning</strong>
                project that predicts customer satisfaction by analyzing relevant features. With data-driven insights, it help
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    The Personal Workout Planner is a Full Stack <strong
                        class="text-violet-400">Next.js</strong
                    >&
                    <strong class="text-violet-400">TailwindCSS</strong>
                    web application, built with <strong class="text-violet-400">Node.js</strong> , that generates personalized workout plans based on user-defined goals and areas to improve. Get stronger, faster, and fitter!"
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
        <p class="mx-auto poppins font-semibold text-lg sm:text-4xl md:text-5xl">
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
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-200 font-semibold"
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
                            >Data Analysis</td
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
        <p class="mx-auto text-3xl">So why not invest?</p>
    </section>
</main>