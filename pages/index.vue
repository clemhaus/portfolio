<template>
  <div>
    <NavBar />
    <Hero />

    <div class="flex flex-col items-center space-y-4 md:flex-row md:justify-center md:space-y-0 mt-8">
      <TimelineSchool />
    </div>

    <div class="flex flex-col items-center space-y-4 md:flex-row md:justify-center md:space-y-0 md:space-x-10 mt-4">
      <CardSafran />
      <CardSyage />
    </div>
    
    <div class="flex flex-col items-center justify-center mt-8">
      <p class="mt-5 mb-1 text-2xl font-semibold leading-7 text-indigo-600 text-center">My current work-study location</p>
      <Google />
    </div>

    <Footer />
  </div>
</template>

<script>
import NavBar from '~/components/NavBar.vue';
import Hero from '~/components/Hero.vue';
import CardSafran from '~/components/CardSafran.vue';
import CardSyage from '~/components/CardSyage.vue';
import TimelineSchool from '~/components/TimelineSchool.vue';
import Google from '~/components/Google.vue';
import Footer from '~/components/Footer.vue';

export default {
  components: {
    NavBar,
    Hero,
    CardSafran,
    CardSyage,
    TimelineSchool,
    Google,
    Footer
  }
}
</script>
