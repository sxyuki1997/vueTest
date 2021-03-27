<template>
  <div id="app">
    <img src="./assets/logo.png">
    <p>{{message}}</p>
    <div class="weibo-wrap">
      <div class="profile">
        <div src="./assets/logo.png"></div>
        <div class="name">由纪昕昕子</div>
        <div class="time">2021/3/26</div>
      </div>
      <div class="txt">今天解放自由啦！接下来指定完整的学习计划，
        坚持去实验室，严格执行！</div>
      <div class='wrap'>
        <div class="list">test</div> 
        <div class="list">test</div>
        <div class="list">test</div>
        <div class="list">test</div>
        <div class="list">test</div>
        <div class="list">test</div>
        <div class="list">test</div>
        <div class="list">test</div>
        <div class="list">test</div>      
      </div>
    </div>

    <!-- <router-view/> -->
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      message: '加油！',
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
  margin-top: 60px;
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
  background-color: antiquewhite;
}
.list {
  width: 100px;
  height: 100px;
  background-color:darkgray;
  margin-left: 10px;
  margin-top: 10px;
}
</style>
