<template>
  <div :class="bigPhotoRight ? 'basic-layout-right' : 'basic-layout-left'">
    <img :src="`/_nuxt/assets/photos/${bigPhotoName}`" alt=""/>
    <p v-if="search">{{ description }}</p>
    <div v-if="search" class="input-container">
        <input type="text" placeholder="Search for a person...">
        <button>Search</button>
    </div>
    <div v-if="!search" class="title-container">
        <h1>{{ title }}</h1>
    </div>
    <p v-if="!search">{{ description }}</p>

    <div v-if="isMini" class="btn-container">
        <button>
            <NuxtLink :to="`${buttonPage}`">{{ buttonText }}</NuxtLink>
        </button>
    </div>

    <div class="img-container">
        <img :src="`/_nuxt/assets/photos/${littlePhotoName}`" alt=""/>
        <!-- <img :src="`/_nuxt/assets/photos/${littlePhoto2Name}`" alt="" /> -->
    </div>
  </div>
</template>

<script>
export default {
  name: "BasicLayout",
  props: {
    bigPhotoName: String, default: "",
    title: String, default: "",
    description: String, default: "",
    buttonPage: String, default: "",
    buttonText: String, default: "",
    littlePhotoName: String, default: "",
    littlePhoto2Name: String, default: "",
    bigPhotoRight: Boolean, default: false,
    isMini: Boolean, default: false,
    search: Boolean, default: false,
  },
};
</script>


<style lang="scss">
@import "~/scss/styles.scss", "~/scss/fonts.scss";
</style>