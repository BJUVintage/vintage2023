<script lang="ts" setup></script>

<template>
  <page-title :title="'Search'" svg="sheep.svg" class="search" svgClass="searchSVG" />
  <basic-layout
    big-photo-name="search-photo.jpg"
    description="Search for people in the 2022-2023 yearbook archives."
    button-page="groups"
    button-text="All Groups"
    little-photo-name="search-2.jpeg"
    search
  ></basic-layout>
</template>

<script>
export default {
  name: "SearchMini",
  }
</script>

<style scoped></style>
