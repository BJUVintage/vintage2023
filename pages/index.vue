<script lang="ts" setup></script>

<template>
    <NuxtLink to="/">
        <img src="~/assets/vintage_desktop.svg" alt="" class="vintage__desktop center">
    </NuxtLink>
    
    <events/>
    <groups/>
    <search/>

</template>

<script>
import events from '~/pages/events.vue'
import groups from '~/pages/groups.vue'
import search from '~/pages/search.vue'

export default {
    components: {
        events,
        groups,
        search,
    }
}
</script>

<style lang="scss">
@import '~/scss/styles.scss', '~/scss/fonts.scss' ;
</style>
