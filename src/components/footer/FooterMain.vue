<template>
    <main class="container d-flex justify-content-between ">
        <div class="d-flex">
            <div class="p-4">
                <div>
                    <h2 class="text-uppercase text-white">dc comics</h2>
                    <ul class="list-unstyled">
                        <li class="text-white" v-for="element in dcComics" :key="element.id">
                            {{ element.text }}
                        </li>
                    </ul>
                </div>
                <div>
                    <h2 class="text-uppercase text-white">shop</h2>
                    <ul class="list-unstyled">
                        <li class="text-white" v-for="element in shop" :key="element.id">
                            {{ element.text }}
                        </li>
                    </ul>
                </div>
            </div>
            <div class="p-4">
                <h2 class="text-uppercase text-white">dc</h2>
                <ul class="list-unstyled">
                    <li class="text-white" v-for="element in dc" :key="element.id">
                        {{ element.text }}
                    </li>
                </ul>
            </div>
            <div class="p-4">
                <h2 class="text-uppercase text-white">sites</h2>
                <ul class="list-unstyled">
                    <li class="text-white" v-for="element in sites" :key="element.id">
                        {{ element.text }}
                    </li>
                </ul>
            </div>
        </div>
        <div>
            <img class="bg-logo" src="img/dc-logo-bg.png" alt="big logo">
        </div>
    </main>
</template>

<script>
    export default {
        name: 'FooterMain',
        data(){
            return{
               dcComics: [
                {
                    id: 1,
                    text: 'Characters'
                },
                {
                    id: 2,
                    text: 'Comics'
                },
                {
                    id: 3,
                    text: 'Movies'
                },
                {
                    id: 4,
                    text: 'TV'
                },
                {
                    id: 5,
                    text: 'Games'
                },
                {
                    id: 6,
                    text: 'Videos'
                },
                {
                    id: 7,
                    text: 'News'
                },
               ],
               shop:[
                {
                    id: 1,
                    text: 'Shop DC'
                },
                {
                    id: 2,
                    text: 'Shop DC Collectibles'
                }
               ],
               dc:[
                {
                    id: 1,
                    text: 'Terms Of Use',
                },
                {
                    id: 2,
                    text: 'Privacy policy (New)',
                },
                {
                    id: 3,
                    text: 'Ad Choices',
                },
                {
                    id: 4,
                    text: 'Advertising',
                },
                {
                    id: 5,
                    text: 'Jobs',
                },
                {
                    id: 6,
                    text: 'Subscriptions',
                },
                {
                    id: 7,
                    text: 'Talent Workshops',
                },
                {
                    id: 8,
                    text: 'CPSC Certificates',
                },
                {
                    id: 9,
                    text: 'Ratings',
                },
                {
                    id: 10,
                    text: 'Shop Help',
                },
                {
                    id: 11,
                    text: 'Contact Us',
                },
               ],
               sites: [
                {
                    id: 1,
                    text: 'DC',
                },
                {
                    id: 1,
                    text: 'MAD Magazine',
                },
                {
                    id: 1,
                    text: 'DC Kids',
                },
                {
                    id: 1,
                    text: 'DC Universe',
                },
                {
                    id: 1,
                    text: 'DC Power Visa',
                },
               ]
            }
        }
    }
</script>

<style lang="scss" scoped>
.bg-logo{
    width: 500px;
    height: 400px;
    object-fit: cover;
}
li{
    font-weight: lighter;
}
</style>