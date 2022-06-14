<template>
    <div class="task-grid">
            <!-- v-for gera as divs com as tarefas.-->
            <TaskList v-for="task in tasks" :key="task.name" :task="task"></TaskList>
        
    </div>

</template>

<script>
import TaskList from './TaskList.vue';
export default {
    componets: { TaskList },
    props: {
        tasks: { type: Array, required: true }
    }
}

</script>

<style>

</style>