<template>
  <!-- 日历组件 -->
  <datePicker
    :options="calendarArr"
    class="calendar"
    @handleClickDay="handleClickDay"
    @handlePrevMonth="handlePrevMonth"
    @handleNextMonth="handleNextMonth"
  />
</template>

<script>
// 日历组件
import datePicker from "./components/data-picker";
export default {
  name: "date-picker",
  data() {
    return {
      calendarArr: {
        type: "combination",
        headStyle: {
          todayBtn: "right",
          combination: "center",
          checkBtn: "right"
        },
        viewStyle: {
          day: "right"
        },
        calendarData: []
      }
    };
  },
  components: {
    datePicker
  },
  methods: {
    handleClickDay() {},
    handlePrevMonth() {},
    handleNextMonth() {}
  }
};
</script>

<style>
</style>
