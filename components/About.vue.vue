<template>
  <div class="relative bg-white">
    <div class="mx-auto max-w-7xl lg:flex lg:justify-between lg:px-8 xl:justify-end">
      <div class="lg:flex lg:w-1/2 lg:shrink-0 xl:absolute xl:inset-y-0 xl:right-1/2 xl:w-1/2">
        <div class="relative h-80 lg:h-full lg:w-full xl:ml-0">
          <img class="relative inset-0 h-full w-full object-contain -mt-10 ml-10" src="./img/cv_portfolio.jpg" alt=""/>
        </div>
      </div>
      <div class="px-6 lg:contents">
        <div class="mx-auto max-w-2xl pb-24 pt-16 sm:pb-32 sm:pt-5 lg:ml-8 lg:mr-0 lg:w-full lg:max-w-lg xl:w-1/2">
          <p class="text-base font-semibold leading-7 text-indigo-600">Welcome to my resume !</p>
          <h1 class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">More about my skills</h1>
          <div class="mt-10 max-w-xl text-base leading-7 text-gray-700 lg:max-w-none">
            <ul role="list" class="mt-8 space-y-8 text-gray-600">
              <li class="flex gap-x-3">
                <CpuChipIcon class="mt-1 h-5 w-5 flex-none text-indigo-600" aria-hidden="true" />
                <span>
                  <strong class="font-semibold text-gray-900">Electronic software.</strong>
                  I have acquired in-depth skills in the use of specialized technical software such as PSpice, Winchem and Wintypon. PSpice is a simulation tool for electrical and electronic circuits, which enabled me to model, analyze and verify the behavior of complex circuits before their physical realization. Winchem, a chemical scheme design and simulation software, helped me to design and optimize chemical processes, taking into account possible interactions and reactions. Finally, Wintypon, a software package for creating printed circuit boards (PCBs), enabled me to design electronic boards by placing components, routing tracks and generating ready-to-use manufacturing files. These skills enable me to efficiently manage the design, simulation and production phases of electronic and chemical projects.
                </span>
              </li>
              <li class="flex gap-x-3">
                <LockClosedIcon class="mt-1 h-5 w-5 flex-none text-indigo-600" aria-hidden="true" />
                <span>
                  <strong class="font-semibold text-gray-900">Software languages.</strong>
                  During my training, I developed programming skills, particularly in C, Java, HTML, PHP, CSS, JSON, Python and NodeJS. These languages and frameworks enable me to build a wide range of applications, from web development using HTML, CSS and JavaScript frameworks to backend development with Python and NodeJS. My knowledge of C and Java further strengthens my ability to understand low-level programming and object-oriented concepts.
                </span>
              </li>
              <li class="flex gap-x-3">
                <ServerIcon class="mt-1 h-5 w-5 flex-none text-indigo-600" aria-hidden="true" />
                <span>
                  <strong class="font-semibold text-gray-900">Databases.</strong>
                  I have developed solid skills in database management and manipulation, including SQL, SQL+, MongoDB, APEX (Oracle) and Cisco. These skills enable me to design, query and optimize relational and non-relational databases. With SQL and SQL+, I can perform complex queries to extract and manipulate data efficiently. My experience with MongoDB gives me the necessary tools to work with NoSQL databases, suitable for applications requiring high flexibility and scalability. APEX (Oracle) enables me to create robust web applications directly from Oracle databases. Finally, my knowledge of Cisco helps me to understand aspects of network management and their integration with databases.
                </span>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { CloudArrowUpIcon, LockClosedIcon, ServerIcon, CpuChipIcon} from '@heroicons/vue/20/solid'
</script>

