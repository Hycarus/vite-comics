<template>
    <div class="footer-top">
        <FooterTop/>
    </div>
    <div class="footer-main">
        <FooterMain/>
    </div>
    <div class="footer-bottom">
        <FooterBottom/>
    </div>
</template>

<script>
import FooterTop from './footer/FooterTop.vue';
import FooterMain from './footer/FooterMain.vue';
import FooterBottom from './footer/FooterBottom.vue';
    export default {
        name: 'FooterApp',
        components: {
            FooterBottom,
            FooterMain,
            FooterTop,
        }
    }
</script>

<style lang="scss" scoped>
@use '../assets/style/main.scss' as *;
    .footer-top{
        background-color: $main_color;
    }
    .footer-main{
        background-image: url(img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    .footer-bottom{
        background-color: $secondary_color;
    }
</style>