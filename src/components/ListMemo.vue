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
  width: 140px;
  height: 140px;
  background-color:rgb(255, 221, 226);
  margin-left: 10px;
  margin-top: 10px; 
  border-radius: 10%;
  display:flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: flex-start;
  overflow: hidden;
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
    font-size: 38px;
    margin-top: 10px;
    color:rgb(175, 153, 252);
    font-weight: 800;

}
</style>