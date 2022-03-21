<template>
    <button @click="this.$emit('btn-click')" :style="{background: color}" class="btn">{{text}}</button>
</template>

<script>
export default {
    name: 'button-item',
    props: {
        text: String,
        color: String
    },
}
</script>

<style>

</style>