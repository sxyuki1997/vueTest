<template>
    <div class="weeklist">
        <div class="week">{{date}}</div>
        <!-- <div class="memo">{{memo}}</div> -->
    </div>
</template>

<script>
export default {
  name: 'Date',
  props: {
      date: {
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
.weeklist {
  width: 140px;
  height: 50px;
  /* background-color:rgb(255, 221, 226); */
  margin-left: 10px;
  /* margin-top: 5px;  */
  border-radius: 10%;
  display:flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: flex-start;
}
.week {
    width: 100%;
    height: 50px;
    font-size: 28px;
    color: rgb(255, 255, 255);
    font-weight: 700;
    margin-top: 10px;
}
</style>