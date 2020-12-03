<template>
  <div id="app">
    <!--displays a series of columns for eachday
    within a week with two hard-coded calendar event-->
    <CalendarWeek />

    <!--displays an input section where users will be able to sumbit
    events in a patricuwlwr day-->
    <CalendarEntry />
  </div>
</template>

<!--Scripts-creates an export of the file with the name of the app-->
<script>
import CalendarWeek from './components/CalendarWeek.vue';
import CalendarEntry from './components/CalendarEntry.vue';

export default {
  name: 'App',
  components: {
    CalendarWeek,
    CalendarEntry
  }
}
</script>


<!--containscustom styling-->
<style lang="scss">
html, body {
  height: 100%;
}
</style>

<style lang="scss" scoped>
#app {
  height: inherit;
  background: #6e6e6e;
  display: flex;
  flex-direction: column;
  align-items: center;
  -webkit-align-items: center;
  justify-content: center;
  -webkit-justify-content: center;
}
</style>
