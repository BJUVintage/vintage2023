<template>
  <div :class="bigPhotoRight ? 'basic-layout-right' : 'basic-layout-left'">
    <img :src="`/_nuxt/assets/photos/${bigPhotoName}`" alt=" "/>

    <!-- if we're using the component for searching -->
    <p v-if="search">{{ description }}</p>
    <div v-if="search" class="input-container">
        <input type="text" placeholder="Search for a person...">
        <button>Search</button>
    </div>
    <div v-if="!search" class="title-container">
        <h1>{{ title }}</h1>
    </div>
    <p v-if="!search">{{ description }}</p>

    <!-- if we're using the component as a preview of a page -->
    <div v-if="isMini" class="btn-container">
        <button>
            <NuxtLink :to="`${buttonPage}`">{{ buttonText }}</NuxtLink>
        </button>
    </div>

    <div class="img-container">
        <img :src="`/_nuxt/assets/photos/${littlePhotoName}`" alt=" "/>
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
    bigPhotoRight: Boolean, default: false,
    isMini: Boolean, default: false,
    search: Boolean, default: false,
  },
};
</script>


<style lang="scss">
@import "~/scss/styles.scss", "~/scss/fonts.scss";
</style>