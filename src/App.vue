<template>
  <header>
    <HeaderApp/>
  </header>
  <section>
    <JumboApp/>
  </section>
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
import JumboApp from './components/JumboApp.vue'
  export default {
    name: 'App',
    components: {
      HeaderApp,
      FooterApp,
      MainApp,
      JumboApp,
    },
    data(){
      return{

      }
    }
  }
</script>

<style lang="scss" scoped>

</style>