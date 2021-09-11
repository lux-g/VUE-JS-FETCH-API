<template>
    <div class="container" v-for="job in jobs" :key="job.id" :jobs="jobs">
        <h4>{{job.name}}</h4>
        <p>{{job.body}}</p>
    </div>
</template>

<script>
    export default {
        data(){
            return {
                jobs: []
            }
        },
        mounted(){
            const getData = async() => {
                const res = await fetch('https://jsonplaceholder.typicode.com/comments')
                const data = await res.json()
                this.jobs = data.slice(0, 10)
                console.log(data)
            }
            getData()
        }
    }
</script>

<style scoped>
.container {
    display: flex;
    flex-direction: column;
    margin: 0px 10vw;
}
.container p {
    margin-bottom: 10px;
}
</style>