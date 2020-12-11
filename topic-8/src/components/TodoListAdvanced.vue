<template>
    <div>
        <h1>Task</h1>
        <Task v-for='t in tasks' v-bind:key='t.id' v-bind:task='t'></Task>
    </div>
</template>

<script>
import Task from "./Task"
export default {
    components:{
        Task
    },
    data:function(){
        return {
            tasks: [
                {
                    id: 1,
                    name: "Wash the car",
                    urgency: "not-urgent",
                    importance:"average",
                    dateDue:"2020-12-31"
                }
            ]
        }
    }
}
</script>
<style scoped>

</style>