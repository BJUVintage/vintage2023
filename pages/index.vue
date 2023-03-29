<script lang="ts" setup></script>

<template>
    <NuxtLink to="/">
        <img src="~/assets/svgs/vintage_desktop.svg" alt="" class="vintage__desktop vintage__center">
    </NuxtLink>

        <p class="center__text">
            Behold, I send you forth as <span>sheep</span><br>
            in the midst of <span>wolves:</span><br>
            be ye therefore wise as <span>serpents,</span><br>
            and harmless as <span>doves.</span>
        </p>
        <p class="verse">Matthew 10:16</p>
    
    <events-mini/>
    <groups-mini/>
    <search-mini/>

</template>

<script>
import EventsMini from '~~/components/EventsMini.vue'

export default {
  components: { EventsMini },
}
</script>

<style lang="scss">
@import '~/scss/styles.scss', '~/scss/fonts.scss' ;
</style>
