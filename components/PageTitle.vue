<template>
    <div class="page__title">
        <h1>{{ title }}</h1>
    </div>
</template>

<script>
export default ({
    name: 'PageTitle',
    props: {
        title: String,
    },
    mounted() {
        this.title;
    }
})
</script>


<style lang="scss">
    @import '~/scss/styles.scss', '~/scss/fonts.scss';
</style>