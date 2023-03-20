<template>
  <div>
    <NuxtPage/>
    <nav style="display:flex; gap:10px">
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="groups">Groups</NuxtLink>
    <NuxtLink to="events">Events</NuxtLink>
    <NuxtLink to="search">Search</NuxtLink>
    </nav>
  </div>
</template>

<style lang="scss">

$bgColor: #204F40;

.index {
  background-color: $bgColor;
}

</style>
