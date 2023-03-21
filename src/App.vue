<template>
  <Navbar />
  <Sidebar/>
  <Banner />
  <Vision />
  <About />
  <Calculators />
  <Footer />
</template>

<script>
import Navbar from './components/nav_bar.vue';
import Banner from './components/banner.vue';
import Vision from './components/vision.vue';
import About from './components/about_us.vue';
import Calculators from './components/calculators.vue';
import Footer from './components/footer.vue';
import Sidebar from './components/sidebar.vue';
export default {
  components : {
    Navbar,
    Sidebar,
    Banner,
    Vision,
    About,
    Calculators,
    Footer,
  }
}
</script>

<style>
  h1 {
    color: white;
    z-index: 9;
  }
</style>