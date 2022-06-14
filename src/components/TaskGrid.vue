<template>
    <div class="task-grid">
        <!-- v-for gera as divs com as tarefas.-->
        <TaskState v-for="task in tasks" :key="task.name" :task="task"></TaskState>
        
    </div>

</template>

<script>
import TaskState from './TaskState.vue'
export default {
    componets: { TaskState },
    props: {
        tasks: { type: Array, required: true }
    }
}

</script>

<style>

</style>