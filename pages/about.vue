<template>
  <div>
    <NavBar />
    <About />
    <Footer />
  </div>
</template>

<script>
import NavBar from '~/components/NavBar.vue';
import About from '~/components/About.vue';
import Footer from '~/components/Footer.vue';

export default {
  components: {
    NavBar,
    About,
    Footer
  }
}
</script>
