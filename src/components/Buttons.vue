<template>
    <button :style="{ background: color }" class="task-btn">{{ title }}</button>
</template>

<script>
export default {
    name: 'Button',
    props: {
        title: String,
        color: String,
    }

}
</script>

<style scoped>
.task-btn {
    background-color: black;
    border: none;
    color: white;
    padding: 10px;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
}
</style>