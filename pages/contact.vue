<template>
  <div>
    <NavBar />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import NavBar from '~/components/NavBar.vue';
import Contact from '~/components/Contact.vue';
import Footer from '~/components/Footer.vue';

export default {
  components: {
    NavBar,
    Contact,
    Footer

  }
}
</script>
