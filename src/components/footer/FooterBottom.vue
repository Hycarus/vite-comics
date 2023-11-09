<template>
    <main class="container">
        <div class="d-flex justify-content-between align-items-center ">
            <button class="btn btn-outline-primary text-uppercase text-white my-button">sign-up now!</button>
            <div class="d-flex align-items-center">
                <h4 class="text-uppercase follow px-3 m-0">follow us</h4>
                <ul class="nav d-flex">
                    <li class="px-2 py-4 " v-for="element in social" :key="element.id">
                        <img :src="element.image" :alt="element.text">
                    </li>
                </ul>
            </div>
        </div>
    </main>
</template>

<script>
    export default {
        name: 'FooterBottom',
        data(){
            return{
                social: [
                    {
                        id: 1,
                        image: 'img/footer-facebook.png',
                        text: 'facebook logo',
                    },
                    {
                        id: 2,
                        image: 'img/footer-twitter.png',
                        text: 'twitter logo',
                    },
                    {
                        id: 3,
                        image: 'img/footer-youtube.png',
                        text: 'youtube logo',
                    },
                    {
                        id: 4,
                        image: 'img/footer-pinterest.png',
                        text: 'pinterest logo',
                    },
                    {
                        id: 5,
                        image: 'img/footer-periscope.png',
                        text: 'periscope logo',
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
@use '../../assets/style/main.scss' as *;
.follow{
    color: $main_color;
}
.my-button{
    border: 1px solid $main_color;
    border-radius: 0;
    height: 50px;
}
</style>