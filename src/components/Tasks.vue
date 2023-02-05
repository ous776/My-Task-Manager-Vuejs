<template>
  
  <div :key="task.id" v-for="task in tasks">
   {{ task.text }}
  </div>
  <!-- <Task   @toggle-reminder="$emit('toggle-reminder', task.id)" @delete-task="$emit('delete-task', task.id)" :task="task"/> -->

</template>

<script>
 /* eslint-disable */
import Task from './Task'
export default {
  name: "Tasks",
  props: {
    tasks: Array,
  },

  components: {
    Task,
  },

  // emits: ['delete-task','toggle-reminder'],

};
</script>