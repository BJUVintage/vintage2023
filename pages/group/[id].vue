<template>
    
    <page-title :title="'Groups'" svg="dove.svg" class="groups" svgClass="groupsSVG" />
    <h1 class="group-title">{{ group.name }}</h1>
    <div class="groups-container">
        <div class="team-name" v-for="(team) in group.content" v-bind:key="team.name">
            <NuxtLink class="team-name" :to="`/group-${group.slug}/team/${team.slug}`">{{ team.name }}</NuxtLink>
        </div>

        <!-- <div class="groups-container" v-for="(team) in group.content" v-bind:key="team.name">
            <NuxtLink class="team-name" :to="`/group/${group.slug}`">{{ team.name }}</NuxtLink>
        </div> -->

        <!-- <NuxtLink class="team-name" v-for="(team) in group.content" v-bind:key="team.name" :to="`/group/${group.slug}`">{{ team.name }}</NuxtLink> -->
        
    </div>
</template>

<script lang="ts">
import { ParsedContent } from '@nuxt/content/dist/runtime/types';

export default {
    name: "GroupPage",
    data() {
        return {
            group: {} as ParsedContent,
        }
    },
    async mounted() {
        const groupSlug = this.$route.params.id;
        this.group = (await queryContent("/groups").find())[0].groups.find((x: ParsedContent) => x.slug.toLowerCase() === groupSlug);
    }
}
</script>