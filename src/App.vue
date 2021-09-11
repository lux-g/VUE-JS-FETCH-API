<template>
  <!-- <Header title="Task Tracker" />
  <Tasks :tasks="tasks" /> -->
  <FetchData />
</template>

<script>
import Header from './components/Header.vue'
import Tasks from './components/Tasks.vue'
import TestBind from './components/TestBind.vue'
import FetchData from './components/FetchData.vue'

export default {
  name: 'App',
  components: {
    FetchData
  },
  data(){
    return {
      tasks: []
    }
  },
  created(){
    this.tasks = [
      {
        id: 1,
        text: 'text one',
        day: 'friday'
      },
            {
        id: 2,
        text: 'text two',
        day: 'saturday'
      },
            {
        id: 3,
        text: 'text three',
        day: 'sunday'
      },
    ]
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
