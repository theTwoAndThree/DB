<template>
  <div class="m-header">
    <el-row>
      <el-col :span="12">
        <nav-bar />
      </el-col>
      <el-col :span="6">
        <search-bar />
      </el-col>
      <el-col :span="3">
        <shop-bar />
      </el-col>
      <el-col :span="3">
        <user />
      </el-col>
    </el-row>
  </div>
</template>
<script>
import navBar from './nav'
import searchBar from './search'
import shopBar from './shop'
import user from './user'
export default {
  components: {
    navBar,
    searchBar,
    shopBar,
    user
  }
}
</script>
<style lang="stylus"></style>