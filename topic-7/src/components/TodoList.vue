<template>
    <div>
       <h1>Todos</h1>
       <div>
           <input type="text" v-model="newTask" placeholder="Enter New Task"/>
           <button v-on:click="addNewTask">Add New Task</button>
       </div>
       <p v-for='t in tasks' v-bind:key='t'>{{t}}<button v-on:click="deleteTask(t)">Delete Task</button></p>
    </div>
</template>
<script>
export default {
    data: function(){
        return{
            'tasks':["Clean the cars",
                     "Wash the clothes",
                     "Pay the bills"
                     ],
            'newTask':''
        }
    },
    methods:{
        addNewTask:function(){
            this.tasks.push(this.newTask)
        },
        deleteTask:function(task){
            let indexToDelete = this.tasks.indexOf(task);
            this.tasks.splice(indexToDelete, 1)
        }
    }
}
</script>
<style scoped>

</style>