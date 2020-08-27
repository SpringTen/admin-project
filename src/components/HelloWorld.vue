<template>
  <el-container style="height: 500px; border: 1px solid #eee">
    <el-header style="text-align: right; font-size: 12px; width： 100%">
      <CommonTop></CommonTop>
    </el-header>
    <el-container>
      <el-aside width="200px" style="background-color: rgb(238, 241, 246)">
        <CommonSider></CommonSider>
      </el-aside>
      <el-container>
        <el-main>
          <CommonContent></CommonContent>
          <!-- <el-pagination background layout="prev, pager, next" :page-count="10" pager-count="3"></el-pagination> -->
        </el-main>
        <el-footer>Footer</el-footer>
      </el-container>
    </el-container>
  </el-container>
</template>

<style>
.el-header, 
.el-footer{
  background-color: rgb(223, 228, 238);
  color: #333;
  text-align: center;
  line-height: 60px;
}

.el-aside {
  background-color: rgb(223, 228, 238);
  color: #333;
  text-align: center;
  line-height: 200px;
  padding-top: 20px;
}

.el-main {
  /* background-color: #e9eef3;rgb(238, 241, 246) */
  background-color: rgb(238, 241, 246);
  color: #333;
  text-align: center;
  line-height: 35px;
  /* height: 1000px; */
}

body > .el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>

<script>
import CommonSider from "./common/CommonSider";
import CommonContent from "./common/CommonContent";
import CommonTop from "./common/CommonTop";
export default {
  components: {
    CommonSider,
    CommonContent,
    CommonTop,
  },
};
</script>