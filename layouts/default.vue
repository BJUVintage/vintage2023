<template>
  <header>
    <nav class="nav">
      <NuxtLink to="events">Events</NuxtLink>
      <NuxtLink to="groups">Groups</NuxtLink>
      <NuxtLink to="search">Search</NuxtLink>
    </nav>
  </header>

  <div class="main-gradient">
    <slot />
  </div>

  <footer>
    <div class="flex-container">
      <div>
        <h2>Built by</h2>
        <h1>The Vintage Staff</h1>
      </div>
      <div class="space-between" />
      <div class="dates">
        <ul>
          <li><a href="http://www.bjuvintage.com/2022/index.html">2022</a></li>
          <li><a href="http://www.bjuvintage.com/2021/index.html">2022</a></li>
          <li><a href="http://www.bjuvintage.com/2020/index.html">2022</a></li>
          <li><a href="http://www.bjuvintage.com/2019/index.html">2022</a></li>
          <br />
          <li><a href="http://www.bjuvintage.com/2018/index.html">2022</a></li>
          <li><a href="http://www.bjuvintage.com/2017/index.html">2022</a></li>
          <li><a href="http://www.bjuvintage.com/2016/index.html">2022</a></li>
          <li><a href="http://www.bjuvintage.com/2015/index.html">2022</a></li>
          <br />
          <li><a href="http://www.bjuvintage.com/2014/index.html">2022</a></li>
        </ul>
      </div>
    </div>
  </footer>
  <div class="green_dingleberry" />
</template>

<style lang="scss">
@import "~/scss/styles.scss", "~/scss/fonts.scss";
</style>

<!-- 
  headers: serif
  body copy: turis

  preliminary -> illustrations -> leaves-illustration
  prelimainry -> interlayout -> styleguide 2.pdf

 -->