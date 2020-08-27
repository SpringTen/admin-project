<template>
  <div>
    <el-table :data="tableData">
      <!-- <el-row>
        <el-col :span="4">
          <div class="grid-content bg-purple-dark"></div>
        </el-col>
      </el-row>-->
      <el-table-column prop="date" label="日期" width="140"></el-table-column>
      <el-table-column prop="name" label="姓名" width="120"></el-table-column>
      <el-table-column prop="age" label="年龄" width="120"></el-table-column>
      <el-table-column prop="address" label="地址" width></el-table-column>
      <el-table-column fixed="right" label="操作" width="150">
        <el-button size="mini" type="primary" @click="handleEdit(scope.$index, scope.row)">
          <i class="el-icon-edit"></i>
        </el-button>
        <el-button size="mini" type="danger" @click="handleDelete(scope.$index, scope.row)">
          <i class="el-icon-delete"></i>
        </el-button>
      </el-table-column>
      <!-- <el-pagination background layout="prev, pager, next" :page-count="10" pager-count="3"></el-pagination> -->
    </el-table>
  </div>
</template>

<script>
export default {
  data() {
    const item = {
      date: "2016-05-02",
      name: "王小虎",
      age: "24",
      address: "上海市普陀区金沙江路 1518 弄",
    };
    return {
      tableData: Array(8).fill(item),
    };
  },
};
</script>

<style>
</style>