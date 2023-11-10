<template>
    <main>
        <div class="container py-3 ">
            <div class="row">
                <MainCard class="col-12 col-md-2 col-lg-2" v-for="(element, index) in comics" :key="index" :img="element.thumb" :title="element.series"/>
            </div>
            
        </div>
    </main>
</template>

<script>
import MainCard from './main/MainCard.vue'
import {comics} from '../data/array.js'
    export default {
        name: 'MainApp',
        components: {
            MainCard,
        },
        data(){
            return{
                comics: comics,
            }
        }
    }
</script>

<style lang="scss" scoped>
@use '../assets/style/main.scss' as *;
    main{
        background-color: $secondary_color;
    }
</style>