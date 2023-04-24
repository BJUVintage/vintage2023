<script lang="ts" setup></script>

<template>
  <page-title :title="'Groups'" svg="dove.svg" class="groups" svgClass="groupsSVG"/>
  <div v-for="(group) in groups" v-bind:key="name">
    <v-btn>{{ group.name }}</v-btn>
  </div>
</template>

<script lang="ts">
import { ParsedContent } from '@nuxt/content/dist/runtime/types';

export default {
  name: "groups",
  data() {
    return {
      groups: [] as ParsedContent[],
    }
  },
  async mounted() {
    this.groups = (await queryContent("/groups").find())[0].groups;
    console.log(this.groups);
  }    
}

</script>

<style scoped></style>
