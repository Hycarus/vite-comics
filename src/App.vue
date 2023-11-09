<template>
  <header>
    <HeaderApp/>
  </header>
  <main>
    <MainApp/>
  </main>
  <footer>
    <FooterApp/>
  </footer>
</template>

<script>
import HeaderApp from './components/HeaderApp.vue';
import FooterApp from './components/FooterApp.vue';
import MainApp from './components/MainApp.vue';
  export default {
    name: 'App',
    components: {
      HeaderApp,
      FooterApp,
      MainApp,
    },
    data(){
      return{

      }
    }
  }
</script>

<style lang="scss" scoped>

</style>