<template style="background:black;">
  <div id="app">
    <div id="backg"></div>
    <center>
      <el-table :data="tableData" style="width: 80%;top:200px;font-size:27px;" size="medium" fit="true" border="true">
        <el-table-column prop="date" label="#" width="40" style="height:50px"></el-table-column>
        <el-table-column prop="name" label="选手姓名" width="180"></el-table-column>
        <el-table-column prop="point1" label="第一轮得分"> </el-table-column>
        <el-table-column prop="point2" label="第二轮观众投票得分"> </el-table-column>
        <el-table-column prop="point3" label="第二轮评委投票得分"> </el-table-column>
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
        date: '1',
        name: '王小虎',
        point1: '20.4',
        point2: '21.4',
        point3: '22.4'
      }, {
        date: '2',
        name: '王小虎',
        point1: '20.4',
        point2: '21.4',
        point3: '22.4'
      }, {
        date: '3',
        name: '王小虎',
        point1: '20.4',
        point2: '21.4',
        point3: '22.4'
      }, {
        date: '4',
        name: '王小虎',
        point1: '20.4',
        point2: '21.4',
        point3: '22.4'
      }, {
        date: '5',
        name: '王小虎',
        point1: '20.4',
        point2: '21.4',
        point3: '22.4'
      }, {
        date: '6',
        name: '王小虎',
        point1: '20.4',
        point2: '21.4',
        point3: '22.4'
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
.el-table__row{
  height: 70px;
}
.has-gutter{
  height: 70px;
}
</style>
