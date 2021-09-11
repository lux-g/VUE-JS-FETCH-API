<template>
    <div class="task-container"> 
        <h1>{{ title }}</h1>
        <Button @click="handleClick" title="ADD TASK" color="black"/>
    </div>
</template>

<script>
import Button from './Buttons.vue'

export default {
    name: "Header",
    components : {
        Button
    },
    props: {
        title: String
    },
    methods: {
        handleClick(){
            console.log('clicked')
        }
    }
}
</script>

<style scoped>
.task-container {
    max-width: 900px;
    margin: auto;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
}
h1 {
    font-size: 40px;
    text-align: center;
}
</style>