<template>
  <div class="nav">
    <div id="logo">
      <a href="/" target="_self" title="首页">
        <img src="https://www.imooc.com/static/img/index/logo.png" alt="首页" />
      </a>
    </div>
    <ul class="nav-item">
      <li class>
        <nuxt-link to="/freeCourse">免费课程</nuxt-link>
      </li>
      <li class>
        <nuxt-link to="/moneyCourse">精品课程</nuxt-link>
      </li>
      <li class>
        <nuxt-link to="/notes">手记</nuxt-link>
      </li>
      <li class>
        <nuxt-link to="/comments">留言区</nuxt-link>
      </li>
    </ul>
  </div>
</template>
<script>
export default {}
</script>
<style lang="css">
.nav {
  position: relative;
  height: 72px;
  font-size: 16px;
}
.nav #logo {
  float: left;
  line-height: 72px;
}
.nav .nav-item {
  float: left;
  list-style: none;
  margin-top: 0px;
}
.nav .nav-item li {
  float: left;
  list-style: none;
  margin: 0px 20px;
  line-height: 72px;
}
</style>