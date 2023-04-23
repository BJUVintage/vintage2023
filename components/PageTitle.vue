<template>
    <div class="section-title">
        <h1>{{ title }}</h1>
        <div class="svg-container">
            <img :src="`/_nuxt/assets/svgs/${svg}`" alt="" :class="svgClass">
        </div>
    </div>
</template>

<script>
export default {
    name: 'PageTitle',
    props: {
        title: String,
        svg: String,
        svgClass: String,
    },
    mounted() {
        this.title;
    },
}
</script>


<style lang="scss">
    @import '~/scss/styles.scss', '~/scss/fonts.scss';
</style>