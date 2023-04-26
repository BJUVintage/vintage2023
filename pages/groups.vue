<script lang="ts" setup></script>

<template>
  <page-title :title="'Groups'" svg="dove.svg" class="groups" svgClass="groupsSVG"/>
  <div class="group-names">
    <div v-for="(group) in groups" v-bind:key="group.name">
          <NuxtLink class="group" :to="`/group/${group.slug}`">{{ group.name }}</NuxtLink>
    </div>
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
