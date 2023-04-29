<template>
  <header>
    <nav>
        <div class="navbar">
          <div class="navbar__logo">
            <NuxtLink to="/">
              <img class="nav-link" src="~/assets/svgs/VINTAGE.svg" alt="">
            </NuxtLink>
          </div>
          <div class="navbar__links">
            <a class="nav-link" href="/events">Events</a>
            <a class="nav-link" href="/groups">Groups</a>
            <a class="nav-link" href="/search">Search</a>
          </div>
        </div>
        <div class="hamburger">
          <div class="bar" />
          <div class="bar" />
          <div class="bar" />
        </div>
    </nav>
  </header>

  <div>
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
      <table>
        <tr>
          <td><a href="http://www.bjuvintage.com/2022/index.html">2022</a></td>
          <td><a href="http://www.bjuvintage.com/2021/index.html">2021</a></td>
          <td><a href="http://www.bjuvintage.com/2020/index.html">2020</a></td>
          <td><a href="http://www.bjuvintage.com/2019/index.html">2019</a></td>
        </tr>
        <tr>
          <td><a href="http://www.bjuvintage.com/2018/index.html">2018</a></td>
          <td><a href="http://www.bjuvintage.com/2017/index.html">2017</a></td>
          <td><a href="http://www.bjuvintage.com/2016/index.html">2016</a></td>
          <td><a href="http://www.bjuvintage.com/2015/index.html">2015</a></td>
        </tr>
        <tr>
          <td><a href="http://www.bjuvintage.com/2014/index.html">2014</a></td>
        </tr>
      </table>
          
          
          
          
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