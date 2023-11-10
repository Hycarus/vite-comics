<template>
    <div class="">
        <img :src="img" class="card-img-top" :alt="title">
        <div class="card-body">
            <p class="text-white py-3 card-text">{{ title.toLocaleUpperCase() }}</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MainCard',
        props: {
            img: String,
            title: String,
        },
        data(){
            return{
            }
        }
    }
</script>

<style lang="scss" scoped>
    img{
        width: 200px;
        height: 250px;
        object-fit: cover;
        object-position: 0 20px;
    }
</style>