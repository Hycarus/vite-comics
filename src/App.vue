<template>
  <header>
    <HeaderApp/>
  </header>
  <footer>
    <FooterApp/>
  </footer>
</template>

<script>
import HeaderApp from './components/HeaderApp.vue';
import FooterApp from './components/FooterApp.vue';
  export default {
    name: 'App',
    components: {
      HeaderApp,
      FooterApp,
    },
    data(){
      return{

      }
    }
  }
</script>

<style lang="scss" scoped>

</style>