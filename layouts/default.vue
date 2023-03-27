<template>
  <div>
    <header>
      <nav class="nav">
        <NuxtLink to="events">Events</NuxtLink>
        <NuxtLink to="groups">Groups</NuxtLink>
        <NuxtLink to="search">Search</NuxtLink>
      </nav>
    </header>

    <div>
        <slot />
    </div>
  </div>
</template>
