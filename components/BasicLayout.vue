<template>
    <img :src="`/_nuxt/assets/photos/${bigPhotoName}`" alt="">
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
    <button>{{ buttonText }}</button>
    <img :src="`/_nuxt/assets/photos/${littlePhotoName}`" alt="">
</template>

<script>
export default {
    name: 'BasicLayout',
    props: {
        bigPhotoName: String,
        title: String,
        description: String,
        buttonText: String,
        littlePhotoName: String,
    },
}
</script>


<style lang="scss">
    @import '~/scss/styles.scss', '~/scss/fonts.scss';
</style>