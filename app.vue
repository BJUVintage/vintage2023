<template>
  <div>
    <NuxtPage/>
    <nav >
      
      <NuxtLink to="/">
      <img src="~/assets/vintage_desktop.svg" alt="" class="vintage__desktop">
      </NuxtLink>

      <NuxtLink to="events">Events</NuxtLink>
      <NuxtLink to="groups">Groups</NuxtLink>
      <NuxtLink to="search">Search</NuxtLink>
    </nav>
  </div>
</template>

<style lang="scss">
@import '~/scss/styles.scss';
@import '~/scss/fonts.scss';
</style>

