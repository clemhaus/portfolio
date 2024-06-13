<template>
  <div class="max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 relative mb-6 min-h-full flex flex-col">
    <a href="#">
      <img class="rounded-t-lg" src="./img/safran.jpg" alt="" />
    </a>
    <div class="p-5 flex-grow">
      <a href="https://www.safran-group.com/fr/developpement-durable/decarboner-aeronautique">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          Digital Supply Chain Engineer - 2023 - 2025
        </h5>
      </a>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
        As a Digital Supply Chain Engineer at Safran SA, I led the Green&Flows project to manage carbon footprint in goods transportation, leveraging skills in Power BI and Python.
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
        Safran SA, the holding company of the Safran Group, is a major French industrial and technological group with an international presence, specializing in the design and production of aircraft engines, helicopters, rockets, aeronautical and defense equipment.
        During this period, I discovered the position of Digital Supply Chain Engineer within the Industrial Purchasing and Performance Department (DIAP), with the main mission of pursuing the Green&Flows project. This project, part of Safran's CSR strategy, aims to manage the carbon footprint associated with the transportation of goods.
        My main tasks were to design the specifications for lot 2 in collaboration with the Information Systems Department (DSIC), to lead weekly meetings (workshops) with various carriers to collect data to determine our carbon footprint, and to process and exploit this data using Power BI.
        These tasks enabled me to put into practice the skills I'd acquired at ESIEA, particularly in databases for PowerBI table management, and in Python for efficient management of information transmitted by suppliers.
        This assignment was a real personal and professional enrichment. I was able to improve my eloquence by leading meetings in French and English with major players in the sector. I gained an in-depth understanding of the sustainability and social responsibility challenges facing Safran and made a significant contribution to strategic projects for the company.
        I also had the opportunity to attend seminars specifically dedicated to the decarbonization project, where various levers were discussed such as technological progress, the development of SAF (sustainable aviation fuels), and modal shift by favoring maritime and road transport for certain air flows.
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
