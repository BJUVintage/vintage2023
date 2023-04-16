<template>
    <div class="section-title">
        <h1>{{ title }}</h1>
        <img src="@/assets/svgs/wolf.svg" alt="">
    </div>
</template>

<script>
export default {
    name: 'PageTitle',
    props: {
        title: String,
    },
    mounted() {
        this.title;
    },
}
</script>


<style lang="scss">
    @import '~/scss/styles.scss', '~/scss/fonts.scss';
</style>