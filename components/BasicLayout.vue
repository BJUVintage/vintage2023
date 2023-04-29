<template>
  <div :class="bigPhotoRight ? 'basic-layout-right' : 'basic-layout-left'">
    <div class="flex-container">
      <!-- if we're using the component for searching -->
      <div v-if="search" class="text-container">
        <p>{{ description }}</p>
        <div class="input-container">
          <input type="text" placeholder="Search for a person...">
          <button>Search</button>
        </div>
      </div>

      <!-- if we're not using the component for searching -->
      <div v-if="!search" class="text-container">
        <h1>{{ title }}</h1>
        <p>{{ description }}</p>
      </div>


      <div class="img-container" v-if="bigPhotoName">
        <img :src="`/_nuxt/assets/photos/${bigPhotoName}`" />
      </div>
    </div>

    <!-- if we're using the component as a preview of a page -->
    <div v-if="isMini" class="btn-container">
      <button>
        <NuxtLink :to="`${buttonPage}`">{{ buttonText }}</NuxtLink>
      </button>
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