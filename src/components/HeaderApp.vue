<template>
    <div class="container">
        <div class="d-flex justify-content-between align-item-center mt-2">
            <div class="">
                <Logo/>
            </div>
            <div>
                <NavBar/>
            </div>
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