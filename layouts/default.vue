<template>
  <div>
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
      <h2>Built by</h2>
      <h1>The Vintage Staff</h1>

      <ul>
        <li><a href="http://www.bjuvintage.com/2022/index.html">2022</a></li>
        <li><a href="http://www.bjuvintage.com/2021/index.html">2021</a></li>
        <li><a href="http://www.bjuvintage.com/2020/index.html">2020</a></li>
        <li><a href="http://www.bjuvintage.com/2019/index.html">2019</a></li>
        <li><a href="http://www.bjuvintage.com/2018/index.html">2018</a></li>
        <br>
        <li><a href="http://www.bjuvintage.com/2017/index.html">2017</a></li>
        <li><a href="http://www.bjuvintage.com/2016/index.html">2016</a></li>
        <li><a href="http://www.bjuvintage.com/2015/index.html">2015</a></li>
        <li><a href="http://www.bjuvintage.com/2014/index.html">2014</a></li>
      </ul>
    </footer>
  </div>
</template>
