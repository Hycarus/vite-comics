<template>
    <div class="d-flex justify-content-evenly ">
        <div class="p-3">
            <Logo/>
        </div>
        <div>
            <NavBar/>
        </div>
    </div>
</template>

<script>
import NavBar from './header/NavBar.vue'
import Logo from './header/Logo.vue'
    export default {
        name: 'HeaderApp',
        components: {
            NavBar,
            Logo,
        },
        
    }
</script>

<style lang="scss" scoped>

</style>