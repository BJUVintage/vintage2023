<template>
    <page-title :title="'Groups'" svg="dove.svg" class="groups" svgClass="groupsSVG" />

    <div class="team-container">
        <h1 class="team-title">{{ team.name }}</h1>
        <ul v-for="(member) in team.members" v-bind:key="member">
            <li class="member">{{ member }}</li>
        </ul>
    </div>
</template>

<script lang="ts">
import { ParsedContent } from '@nuxt/content/dist/runtime/types';
export default {
    name: "GroupPage",
    data() {
        return {
            group: {} as ParsedContent,
            team: {} as ParsedContent,
        }
    },
    async mounted() {
        const groupSlug = this.$route.params.id;
        const teamSlug = this.$route.params.team;
        this.group = (await queryContent("/groups").find())[0].groups.find((x: ParsedContent) => x.slug.toLowerCase() === groupSlug);
        this.team = this.group.content.find((x: ParsedContent) => x.slug.toLowerCase() === teamSlug);
        console.log(this.team);
    }
}
</script> 