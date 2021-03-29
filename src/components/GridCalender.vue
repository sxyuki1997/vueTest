<template>
<div class="calender">
    <div class='wrap'>
        <div class="list-wrap" 
        v-for="content in contents" :key="content">
            <list-memo 
                :month="content.month" 
                :memo="content.memo">
            </list-memo>
        </div>
    </div>
</div>

</template>

<script>
import ListMemo from './ListMemo'
import Date from './Date'
export default {
  name: 'GridCalender',
  components: { ListMemo, Date},
  data () {
    return {
        contents: [{
            month: '1月', 
            memo: '1月已经过去！'
        },{
            month: '2月', 
            memo: '2月已经过去!'
        },{
            month: '3月', 
            memo: '巩固基础！'
        },{
            month: '4月', 
            memo: ''
        },{
            month: '5月', 
            memo: ''
        },{
            month: '6月', 
            memo: 'C'
        },{
            month: '7月', 
            memo: ''
        },{
            month: '8月', 
            memo: 'B'
        },{
            month: '9月', 
            memo: ''
        }, {
            month: '10月', 
            memo: ''
        }, {
            month: '11月', 
            memo: ''
        }, {
            month: '12月', 
            memo: ''
        }],
        list: []
    } 
  },
  props: ['memo', 'month', 'date']
}
</script>

<style>
.calender {
    display: flex;
    justify-content: center;
    align-items: flex-start;
}
.wrap {
  width: 970px;
  height: 1000px;
  display: flex;
  justify-content: flex-start;
  align-content: flex-start;
  flex-wrap: wrap;
}
.list-wrap {
    flex: 1;
    position: relative;

}

</style>