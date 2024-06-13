<template>
  <div class="max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 relative mb-6 min-h-full flex flex-col">
    <a href="#">
      <img class="rounded-t-lg" src="./img/syage4.png" alt="" />
    </a>
    <div class="p-5 flex-grow">
      <a href="https://www.syage.org/a-votre-service/l-yerres-en-direct/">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          Remote management and information processing engineer - 2023 - 2021
        </h5>
      </a>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
        At SyAGE, I served as a Remote Management Engineer, implementing a hydraulic measuring station, automating reports with business intelligence tools, and gaining experience in remote supervision and data backup.
      </p>
      <button @click="toggleText" class="inline-flex items-center px-3 py-2 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
        Read more
        <svg class="rtl:rotate-180 w-3.5 h-3.5 ms-2" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10">
          <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 5h12m0 0L9 1m4 4L9 9"/>
        </svg>
      </button>
    </div>
    <div v-if="showText" class="p-5">
      <p class="text-sm text-gray-500 dark:text-gray-400">
        I did my work-study in a mixed syndicate called "SyAGE". 
        The SyAGE intervenes in the sectors of sanitation and hydraulics, it has many competences in water management and sanitation. 
        It is also responsible for the maintenance and development of the Yerres and its tributaries. 
        It deals with the control of rainwater and runoff, flood control, pollution control, and the protection and conservation of surface and groundwater. 
        I discovered the position of Remote Management Engineer in the Remote Management and Information Processing Department. 
        The remote management engineer's mission is to ensure the supervision and operation of the department's remote installations, as well as the programming and development of sites to be connected to the supervision. 
        He/she must process the data, provide the necessary assistance to the remote management user services and participate in crisis management. 
        The supervision allows to manage remotely different structures. I had to implement a hydraulic measuring station and automating reports on a tool of business intelligence.
        The design of these reports allowed to observe the activity of the various works. In the framework of my mission, I was brought to make field activities like the change of batteries (rain gauges, radar probe, ultrasound probe) and the reading of water heights on several sites. 
        I also performed the semi-annual backup of our operator stations and the servers of the remote management and information processing department. The semi-annual backup was very important because it allowed us to keep our data safe. 
        This work experience allowed me to understand the architecture of remote management (communication protocols, etc.). It also allowed me to acquire good bases in automatism and industrial data processing.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showText: false,
    };
  },
  methods: {
    toggleText() {
      this.showText = !this.showText;
    },
  },
};
</script>
