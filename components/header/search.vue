<template>
  <div class="search">
    <div class="search-area">
      <input type="text" class="search-input" placeholder="请输入要搜索的内容" />
      <div class="show-hide">
        <i class="el-icon-search"></i>
      </div>
    </div>
  </div>
</template>
<script>
export default {}
</script>
<style lang="css">
.search {
  position: relative;
  height: 72px;
  box-sizing: border-box;
}
.search .search-area {
  display: inline;
}
.search .search-input {
  float: left;

  border: none;
  outline: medium;
  height: 46px;
  font-size: 12px;
  margin-top: 12px;
  /* margin-bottom: 20px; */
  padding: 12px 0;
  border-bottom: 1px solid rgb(145, 145, 145);
}
.search .search-input:focus {
  border-bottom: 1px solid red;
}
.search .show-hide {
  float: left;
  cursor: pointer;
  position: relative;
  /* position: absolute; */
}
.search .show-hide:hover {
  overflow: hidden;
}
/* .search .show-hide .icon-wrapper {
  width: 20px;
  height: 20px;
  z-index: 1;
} */

.search .show-hide i {
  margin-left: 2px;
  margin-top: 28px;
}
.search .show-hide i:hover {
  /* background-color: red;
  opacity: 0.3;
  border-radius: 10px;
  display: inline-block;
  width: 25px;
  height: 25px;
  z-index: 5; */
  filter: drop-shadow(20px 0 red);
  position: relative;
  left: -20px;
}
</style>
