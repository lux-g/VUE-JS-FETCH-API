<template>
    <h2>{{ count }}</h2>
    <button @click="increment" class="increment">increment</button>
    <button @click="decrement" class="decrement">decrement</button>
</template>

<script>
export default {
    data() {
        return {
            count: 0,
        }
    },
    methods: {
        increment(){
            this.count += 1
        },
        decrement(){
            this.count -= 1
        }
    }
}
</script>