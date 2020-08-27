<template>
  <div>
    <el-dropdown>
      <i class="el-icon-setting" style="margin-right: 15px"></i>
      <el-dropdown-menu slot="dropdown">
        <el-dropdown-item>查看</el-dropdown-item>
        <el-dropdown-item>新增</el-dropdown-item>
        <el-dropdown-item>删除</el-dropdown-item>
      </el-dropdown-menu>
    </el-dropdown>
    <span>王小虎</span>
    <el-avatar :src="circleUrl">
      <img src="../../assets/logo.jpg" />
    </el-avatar>
  </div>
</template>

<style scoped>
.el-avatar {
  /* height: 100px; */
  vertical-align: middle;
  margin-left: 18px;
}
</style>
<script>
  export default {
    data () {
      return {
        // circleUrl: "https://cube.elemecdn.com/0/88/03b0d39583f48206768a7534e55bcpng.png",
      }
    }
  }
</script>