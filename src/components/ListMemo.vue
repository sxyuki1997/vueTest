<template>
    <div class="list">
        <div class="month">{{month}}</div>
        <div class="memo">{{memo}}</div>
    </div>
</template>

<script>
export default {
  name: 'GridCalender',
  props: {
      month: {
          type: String,
          default: ''
      },
      memo: {
          type: String,
          default: ''
      }
  },
  data () {
    return {
    } 
  }
}
</script>

<style>
.list {
  width: 230px;
  height: 230px;
  background-color:rgb(255, 221, 226);
  margin-left: 10px;
  margin-top: 10px; 
  border-radius: 10%;
  display:flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: flex-start;
  overflow: hidden;
  transition: flex .4s ease;
}
.list:hover {
    flex: 2;
}
.month {
    width: 100%;
    height: 50px;
    font-size: 34px;
    color: rgb(243, 63, 87);
    font-weight: 700;
    margin-top: 10px;
    background-color:rgb(254, 255, 248);
}
.memo {
    width: 300px;
    height: 200px;
    font-size: 20px;
    margin-top: 10px;
    color:rgb(83, 83, 83);

}
</style>