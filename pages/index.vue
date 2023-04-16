<script lang="ts" setup></script>

<template>
    <div class="VINTAGE">
        <img src="~/assets/svgs/VINTAGE-title.svg" alt="" />
        <div class="trapezoid">
            <h2 class="center">2023</h2>
        </div>
    </div>

  <p class="verse">
    Behold, I send you forth as <span>sheep</span><br />
    in the midst of <span>wolves:</span><br />
    be ye therefore <span>wise</span> as serpents,<br />
    and <span>harmless</span> as doves.
  </p>
  <p id="reference">Matthew 10:16</p>

  <div class="spacer" />

  <events-mini />
  <groups-mini />
  <search-mini />
</template>

<script>
import EventsMini from "~~/components/EventsMini.vue";

export default {
  components: { EventsMini },
};
</script>

<style lang="scss">
@import "~/scss/styles.scss", "~/scss/fonts.scss";
</style>
