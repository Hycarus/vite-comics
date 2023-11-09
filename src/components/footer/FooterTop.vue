<template>
    <main class="container">   
        <ul class="nav justify-content-center p-3">
            <li class="nav-item p-3 " v-for="(element, index) in footerTopImage" key="index">
                <img :src="element.image" alt="">
            </li>
        </ul>
    </main>
</template>

<script>
    export default {
        name: 'Footertop',
        data(){
            return{
                footerTopImage: [
                    {
                        id: 1,
                        image: 'img/buy-comics-digital-comics.png',
                    },
                    {
                        id: 2,
                        image: 'img/buy-comics-merchandise.png',
                    },
                    {
                        id: 3,
                        image: 'img/buy-comics-subscriptions.png',
                    },
                    {
                        id: 4,
                        image: 'img/buy-comics-shop-locator.png',
                    },
                    {
                        id: 5,
                        image: 'img/buy-dc-power-visa.svg',
                    },
                ]
            }
        },
    }   
</script>

<style lang="scss" scoped>
@use '../../assets/style/main.scss' as *;
   
</style>