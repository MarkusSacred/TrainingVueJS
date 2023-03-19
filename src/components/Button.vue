<template>
    <button class="btn" :style="{background: color}">{{ title }}</button>
</template>

<script>
export default {
    name: 'Button',
    props:{
        title: String,
        color: String
    }
    }
</script>

<style scoped>
    .btn {
        margin-left: 20px;
        margin-right: 0px;
    }
</style>