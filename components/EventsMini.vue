<script lang="ts" setup></script>

<template>
  <page-title title="Events" svg="wolf.svg" class="events" svgClass="eventSVG" />
  <basic-layout
    big-photo-name="/events/welcome-week-1.jpeg"
    title="Welcome Week"
    description="Welcome Week introduces incoming freshmen as well as
returning students to University life. The 2022-23 welcome
theme—OWN IT—challenged students to accept personal
responsibility for the academic year and their future. The
week sponsors unique activities, including “meet and
greet” for majors, student orientation, and international
student orientation to acclimate students to their programs,
faculty, and peers. From check-in to opening exercises,
Welcome Week equips students for a successful year."
    button-page="events"
    button-text="All Events"
    big-photo-right
    is-mini
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
