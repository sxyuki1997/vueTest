<template>
  <div id="app">
    <div class="header">
      <h1 style="color: white;">2021年度计划！</h1>
      <h2 style="color: white;"   >加油！</h2>
    </div>
    <div class="content">
      <div class="left"></div>
      <!-- <div class="header"></div> -->
      <!-- <h1 style="color: lightpink; margin-top: 0px;" >808 四月值日表</h1> -->
      <!-- <router-view/> -->
      <!-- <img src="./assets/logo.png"> -->
      <!-- <h3 style="color: grey">{{message}}</h3> -->
      <!-- <flex-box></flex-box> -->
      <div class="middle">
        <grid-calender></grid-calender>
      </div>
      <div class="right"></div>
    </div>
    <div class="footer">
      <h5 style="margin-top: 0px; color: white">为了能够有更好的基础加油！</h5>
    </div>

  </div>
</template>

<script>
import FlexBox from './components/FlexBox'
import GridCalender from './components/GridCalender'
export default {
  components: { FlexBox, GridCalender },
  name: 'App',
  data () {
    return {
      message: '小可爱们加油一起打扫吧！',
      list: [
        'Foo',
        'Bar'
      ]
    } 
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}

.header {
  background-color: rgba(240, 12, 54, 0.233);
  width: 100%;
  height: 200px;
}
.content {
  width: 100%;
  height: 100%;
  background-color: linen;
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
  flex: wrap;
}
.left {
  width: 200px;
  height: 1000px;
  /* background-color: rgb(255, 243, 218); */
}
.right {
  width: 200px;
  height: 1000px;
  /* background-color: rgb(255, 243, 218); */
  margin-right: 0px;
}
.middle {
  width: 100%;
  height: 1000px;
  /* background-color: orange; */
}

.weibo-wrap {
  height: 500px;
  width: 350px;
  display: flex;
  align-content: flex-start;
  justify-content: flex-start;
  flex-wrap: wrap;
}
.profile {
  height: 80px;
  width: 350px;
  display: flex;
  justify-content: space-between;
  align-content: flex-start;
}
.pic {
  width: 70px;
  height: 70px;
  background-color: goldenrod;
  margin-left: 10px;
}
.name {
  width: 100px;
  height: 10px;
  margin-left: -50px;
  font-size: 12px;
  margin-top: 5px;
}
.time {
  width: 80px;
  height: 10px;
  margin-top: 10px;
  font-size: 12px;
}
.txt {
  width: 300px;
  height: 50px;
  font-size: 10px;
  margin-left: 10px;
  text-align: start;
}
.wrap {
  width: 350px;
  height: 350px;
  display: flex;
  justify-content: flex-start;
  align-content: flex-start;
  flex-wrap: wrap;
  /* background-color: antiquewhite; */
}
.list {
  width: 100px;
  height: 100px;
  background-color:darkgray;
  margin-left: 10px;
  margin-top: 10px;
}
.footer {
  width: 100%;
  height: 100px;
  background-color: rgb(126, 126, 125);
}
</style>
