<script lang="ts" setup></script>

<template>
  <page-title :title="'Events'" class="events" />
  <basic-layout
    big-photo-name="feelsgoodman.jpg"
    title="Rush"
    description="Some random text about how rush this year was the best thing ever and this is really just filler text I need something here so it looks more complete."
    button-text="some Text"
    little-photo-name="feelsgoodman.jpg"
  ></basic-layout>
</template>

<script>
export default {
  name: "EventsMini",
};
</script>

<style lang="scss">
@import "~/scss/styles.scss", "~/scss/fonts.scss";
</style>
