<template>
    <div v-for="task in tasks" :key="task.id">
        <Task />
    </div>
</template>

<script>
import Task from './Task.vue'

export default {
    name: 'Tasks',
    props: {
        tasks: Array
    },
    components: {
        Task,
    }
}
</script>