<template>
  <div class="group-container">
    <h1 class="group-title">{{ groupTitle }}</h1>
        <ul>
            <li>nameeeee</li>
            <li>nameeeee</li>
            <li>nameeeee</li>
            <li>nameeeee</li>
            <li>nameeeee</li>
        </ul>

        <div class="flex-container">
            <div class="big-photo"></div>
        </div>

        <div class="flex-container">
            <div  class="small-photo"/>
            <div  class="small-photo"/>
            <div  class="small-photo"/>
        </div>
  </div>
</template>

<script>
export default {
  name: "Group",
  data() {
  },
  props: {
    groupTitle: String,
    names: Array,
  },
  mounted() {
    this.groupTitle;
    this.names;
  },
};
</script>


<style lang="scss">
@import "~/scss/styles.scss", "~/scss/fonts.scss";
</style>