<template>
    <div class="testing">
        <h1>TEST COMPONENT</h1>
        <p>this is a test page</p>
        <input type="text">
        <button @click="handleClick" ref="btn">click me</button>
    </div>
</template>

<script>
export default {
    name: "Test",
    methods: {
        handleClick(){
            console.log(this.$refs.btn)
            this.$refs.btn.classList.toggle('active')
        }
    }
}
</script>

<style scoped>
h1 {
    font-size: 40px;
}
.active {
    background: red;
}
</style>