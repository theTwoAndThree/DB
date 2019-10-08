<template>
  <div class="user">
    <!-- <template v-if="user">
      欢迎您，
      <span class="username">{{ }}</span>
      [
      <nuxt-link to="/exit">退出</nuxt-link>]
    </template>
    <template v-else>
      <nuxt-link to="/login" class="login">立即登录</nuxt-link>
      <nuxt-link class="register" to="/register">注册</nuxt-link>
    </template>-->
    <ul>
      <li>
        <nuxt-link to="/login" class="login">立即登录</nuxt-link>
      </li>
      <li>
        <span>/</span>
      </li>
      <li>
        <nuxt-link class="register" to="/register">注册</nuxt-link>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    user: ''
  }
}
</script>
<style lang="css">
.user {
  display: inline-block;
  height: 72px;
  line-height: 72px;
  font-size: 14px;
}
ul {
  list-style: none;
}
li {
  list-style: none;
  float: right;
  margin: 0 8px;
}
a:hover {
  color: red;
}
</style>