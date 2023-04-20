<template>
  <header>
    <nav class="nav">
        <div><img src="~/assets/svgs/VINTAGE.svg" alt=""></div>
        <div></div>
        <div><NuxtLink to="events">Events</NuxtLink></div>
        <div><NuxtLink to="groups">Groups</NuxtLink></div>
        <div><NuxtLink to="search">Search</NuxtLink></div>

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
        <h5>© Copyright 2022 Bob Jones University</h5>
      </div>
      <div class="space-between" />
      <div class="dates">
      <h3>PREVIOUS YEARS</h3>
        <ul>
          <li><a href="http://www.bjuvintage.com/2022/index.html">2022</a></li>
          <li><a href="http://www.bjuvintage.com/2021/index.html">2021</a></li>
          <li><a href="http://www.bjuvintage.com/2020/index.html">2020</a></li>
          <li><a href="http://www.bjuvintage.com/2019/index.html">2019</a></li>
          <br />
          <li><a href="http://www.bjuvintage.com/2018/index.html">2018</a></li>
          <li><a href="http://www.bjuvintage.com/2017/index.html">2017</a></li>
          <li><a href="http://www.bjuvintage.com/2016/index.html">2016</a></li>
          <li><a href="http://www.bjuvintage.com/2015/index.html">2015</a></li>
          <br />
          <li><a href="http://www.bjuvintage.com/2014/index.html">2014</a></li>
        </ul>
      </div>
    </div>
  </footer>
  <!-- <div class="green_dingleberry" /> -->
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