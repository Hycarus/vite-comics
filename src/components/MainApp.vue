<template>
    <main>
        
        <div class="container py-3 position-relative">
            <h5 class="text-uppercase text-white current-series px-4 py-2 ">
                current series
            </h5>
            <div class="row">
                <MainCard class="col-12 col-md-2 col-lg-2" v-for="(element, index) in comics" :key="index" :img="element.thumb" :title="element.series"/>
            </div>
            <div class="text-center">
                <button class="btn text-uppercase text-white border my-button px-5">load more</button>
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
    .my-button{
        border-radius: 0;
        border-color: $main_color!important;
        background-color: $main_color;
    }
    .current-series{
        background-color: $main_color;
        border-radius: 0;
        position: absolute;
        top: -20px;
        left: -10px;
        font-weight: bolder;
    }
</style>