<template>
    <Header />
    <router-view/>
    <Footer />
</template>

<script>
import './style/global.css'
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Cliente from './services/clientes'

export default {
  components: {
    Header,
    Footer
  }
} 

</script>

<style>


</style>
