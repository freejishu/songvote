<template style="background:black;">
  <div id="app">
    <div id="backg"></div>
    <center>
      <el-table :data="tableData" style="width: 80%;top:200px">
        <el-table-column
          prop="date"
          label="日期"
          width="180">
        </el-table-column>
        <el-table-column
          prop="name"
          label="姓名"
          width="180">
        </el-table-column>
        <el-table-column
          prop="address"
          label="地址">
        </el-table-column>
      </el-table>
    </center>
    
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data() {
    return {
      tableData: [{
        date: '2016-05-02',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1518 弄'
      }, {
        date: '2016-05-04',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1517 弄'
      }, {
        date: '2016-05-01',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1519 弄'
      }, {
        date: '2016-05-03',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1516 弄'
      }]
    }
  },
  beforeCreate () {
      document.querySelector('body').setAttribute('style', 'margin:0px')
},
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
  height: 100%
}
#backg{
  background:url(https://pic.rmb.bdstatic.com/bjh/9ab1edefff4e6144aca1a5745b351358.png) no-repeat fixed center;
  -webkit-filter: brightness(50%); /* Chrome, Safari, Opera */
  filter: brightness(50%);
  float:left;
  width:100%;
  height:100%;
  position:absolute;
  z-index: -1;
}
.body{
  margin:0;
}
</style>
