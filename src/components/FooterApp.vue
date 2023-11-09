<template>
    <div class="footer-top">
        <FooterTop/>
    </div>
    <div>
        <FooterMain/>
    </div>
    <div>
        <FooterMain/>
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
</style>