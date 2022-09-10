<template>
  <el-card class="box-card" style="left: 25%">
    <img src="img/bc.png">
    <h3>Blockchain</h3>
  </el-card>
  <el-card class="box-card" style="left: 45%">
    <img src="img/dc.png" style="width: 150%;height: 150%">
    <h3>Docker</h3>
  </el-card>
  <el-card class="box-card" style="left: 65%">
    <img src="img/go.png">
    <h3>Golang</h3>
  </el-card>

</template>

<script>
export default {
  name: "page2Bottom"
}
</script>

<style scoped>
el-card{
  display: inline;
  position: fixed;
  bottom: 20%;
}
</style>