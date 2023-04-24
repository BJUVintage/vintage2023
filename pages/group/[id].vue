<template>
    <div>
        <h1>{{ group.name }}</h1>
        <div v-for="(team) in group.content">
            <p>{{ team.name }}</p>
        </div>
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