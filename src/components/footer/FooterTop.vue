<template>
    <main class="container">   
        <ul class="nav py-3">
            <li class="my-3 d-flex align-items-center justify-content-center" v-for="(element, index) in footerTopImage" :key="index">
                <div class="text-center">
                    <img class="my-img-w" :src="element.image" :alt="element.text">
                </div>
                <div class="text-uppercase text-white my-text">{{ element.text }}</div>
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
                        text: 'digital comics',
                    },
                    {
                        id: 2,
                        image: 'img/buy-comics-merchandise.png',
                        text: 'dc merchandise',
                    },
                    {
                        id: 3,
                        image: 'img/buy-comics-subscriptions.png',
                        text: 'subscriptions',
                    },
                    {
                        id: 4,
                        image: 'img/buy-comics-shop-locator.png',
                        text: 'comic shop locator',
                    },
                    {
                        id: 5,
                        image: 'img/buy-dc-power-visa.svg',
                        text: 'dc power visa',
                    },
                ]
            }
        },
    }   
</script>

<style lang="scss" scoped>
@use '../../assets/style/main.scss' as *;

ul > li:last-child {
    img{
        width: 80px !important;
    }
    div:last-child{
        padding: 0 20px;
    }
    div:first-child{
        padding-left: 20px;
    }
}
.my-img-w{
    width: 40%;
}
</style>