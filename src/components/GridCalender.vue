<template>
<div class="calender">
    <div class='wrap'>
        <div v-for="date in dates" :key="date">
            <date 
                :date="date.week">
            </date>
        </div>
        <div v-for="content in contents" :key="content">
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
        dates: [{
            week: 'SUN'
        },{
            week: 'MON'
        },{
            week: 'TUE'
        },{
            week: 'WED'
        },{
            week: 'THU'
        },{
            week: 'FRI'
        },{
            week: 'SAT'
        }],
        contents: [{
            month: '', 
            memo: ''
        }, {
            month: '', 
            memo: ''
        }, {
            month: '', 
            memo: ''
        }, {
            month: '01', 
            memo: ''
        },{
            month: '02', 
            memo: 'B'
        },{
            month: '03', 
            memo: ''
        },{
            month: '04', 
            memo: 'A'
        },{
            month: '05', 
            memo: ''
        },{
            month: '06', 
            memo: ''
        },{
            month: '07', 
            memo: 'C'
        },{
            month: '08', 
            memo: ''
        },{
            month: '09', 
            memo: 'B'
        },{
            month: '10', 
            memo: ''
        },{
            month: '11', 
            memo: 'A'
        },{
            month: '12', 
            memo: ''
        },{
            month: '13', 
            memo: ''
        },{
            month: '14', 
            memo: 'C'
        },{
            month: '15', 
            memo: ''
        },{
            month: '16', 
            memo: 'B'
        },{
            month: '17', 
            memo: ''
        },{
            month: '18', 
            memo: 'A'
        },{
            month: '19', 
            memo: ''
        },{
            month: '20', 
            memo: ''
        },{
            month: '21', 
            memo: 'C'
        },{
            month: '22', 
            memo: ''
        },{
            month: '23', 
            memo: 'B'
        },{
            month: '24', 
            memo: ''
        },{
            month: '25', 
            memo: 'A'
        },{
            month: '26', 
            memo: ''
        },{
            month: '27', 
            memo: ''
        },{
            month: '28', 
            memo: 'C'
          },{
            month: '29', 
            memo: ''
        },{
            month: '30', 
            memo: 'B'
        } ],
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
  width: 1060px;
  height: 810px;
  display: flex;
  justify-content: flex-start;
  align-content: flex-start;
  flex-wrap: wrap;
  background-color:lightpink;
  border-radius: 1%;
}

</style>