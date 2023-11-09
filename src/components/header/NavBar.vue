<template>
    <ul class="nav justify-content-center pt-5">
        <li class="nav-item" v-for="(element, index) in menu" :key="index">
            <a href="#" class="nav-link text-black text-uppercase pb-4" :class="{'border-active': isActive(element.id)}" @click="activeMenu = element.id">{{element.text}}</a>
        </li>
    </ul>
</template>

<script>
    export default {
        name: 'NavBar',
        data(){
            return{
                activeMenu: 2,
                menu: [
                    {
                        id: 1,
                        text: 'Characters',
                        visible: false,
                    },
                    {
                        id: 2,
                        text: 'Comics',
                        visible: true,
                    },
                    {
                        id: 3,
                        text: 'Movies',
                        visible: false,
                    },
                    {
                        id: 4,
                        text: 'TV',
                        visible: false,
                    },
                    {
                        id: 5,
                        text: 'Games',
                        visible: false,
                    },
                    {
                        id: 6,
                        text: 'Collectibles',
                        visible: false,
                    },
                    {
                        id: 7,
                        text: 'Videos',
                        visible: false,
                    },
                    {
                        id: 8,
                        text: 'Fans',
                        visible: false,
                    },
                    {
                        id: 9,
                        text: 'News',
                        visible: false,
                    },
                    {
                        id: 10,
                        text: 'Shop',
                        visible: false,
                    },
                ]
            }
        },
        methods: {
            isActive(id){
                return id === this.activeMenu ? true : false;
            },
            getIndex(id, array){
                return array.findIndex((el) => el.id === id);
            }
        },
        computed: {
            activeIndex(){
                return getIndex(this.activeMenu, this.menu)
            }
        }
    }
</script>

<style lang="scss">
@use '../../assets/style/main.scss' as *;
    .border-active{
        border-bottom: 10px solid $main_color;
        color: $main_color !important;
    }
</style>