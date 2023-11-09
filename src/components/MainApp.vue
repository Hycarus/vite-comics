<template>
    <main>
        <div class="container">
            <h1 class="text-white p-4">
                --&gt; Content goes here &lt;--
            </h1>
        </div>
    </main>
</template>

<script>
    export default {
        name: 'MainApp',
    }
</script>

<style lang="scss" scoped>
@use '../assets/style/main.scss' as *;
    main{
        background-color: $secondary_color;
    }
</style>