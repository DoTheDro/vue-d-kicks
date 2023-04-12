<script>
  import Navbar from './components/Navbar.vue'
  import Hero from './components/Hero.vue'
  import AboutUs from './components/AboutUs.vue'
  import Shop from './components/Shop.vue'
  import Reservations from './components/Reservations.vue'
  import Footer from './components/Footer.vue'

  export default {
    components: { Navbar, 
      Hero, 
      AboutUs, 
      Shop, 
      Reservations, 
      Footer }
  }
</script>

<template>
  <Navbar />
  <main>
    <Hero />
    <AboutUs />
    <Shop />
    <Reservations />
  </main>
  <Footer />
</template>
