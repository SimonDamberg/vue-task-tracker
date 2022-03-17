<template>
    <header>
        <h1>{{title}}</h1>
        <Button text="Add Task" color="green"/>
    </header>
</template>

<script>
import Button from './Button.vue' 

export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'header-item',
    props: {
        title: String
    },
    components: {
        Button
    }
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
