<template>
    <header>
        <h1>{{title}}</h1>
        <Button @btn-click="$emit('toggle-add-task')" :text="showAddTasks ? 'Close' : 'Add Task'" :color="showAddTasks ? 'red' : 'green'"/>
    </header>
</template>

<script>
import Button from './Button.vue' 

export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'header-item',
    props: {
        title: String,
        showAddTasks: Boolean
    },
    components: {
        Button
    },
    emits: ['toggle-add-task']
}
</script>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 30px;
}
</style>
