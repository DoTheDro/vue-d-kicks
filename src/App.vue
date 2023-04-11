<script>
  import Navbar from './components/Navbar.vue'
  import Hero from './components/Hero.vue'
  import AboutUs from './components/AboutUs.vue'
  import Shop from './components/Shop.vue'

  export default {
    components: { Navbar, Hero, AboutUs, Shop }
  }
</script>

<template>
  <Navbar />
  <main>
    <Hero />
    <AboutUs />
    <Shop />
  </main>
</template>
