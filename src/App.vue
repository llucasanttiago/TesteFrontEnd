<template>
    <Navbar />
    <router-view/>
    <Footer />
</template>

<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';
import Cliente from './services/clientes'

export default {
  components: {
    Navbar,
    Footer
  }
} 

</script>

<style>


</style>
