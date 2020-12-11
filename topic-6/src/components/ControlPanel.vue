<template>
  <div>
      <div class="row">
          <Box v-bind:bgColor="box1Color" content="1" v-on:reset_backgroundcolor="resetBox1"></Box>
          <Box v-bind:bgColor="box2Color" content="2" v-on:reset_backgroundcolor="resetBox2"></Box>
          <Box v-bind:bgColor="box3Color" content="3" v-on:reset_backgroundcolor="resetBox3"></Box>
      </div>
      <h1>Select box color</h1>
      <div>
       <label>Box 1 </label>
       <select v-model="box1Color">
          <option value="red">Red</option>
          <option value="green">Green</option>
          <option value="blue">Blue</option>
       </select>
      </div>
      <div>
       <label>Box 2 </label>
       <select v-model="box2Color">
          <option value="red">Red</option>
          <option value="green">Green</option>
          <option value="blue">Blue</option>
       </select>
      </div>
      <div>
       <label>Box 3 </label>
       <select v-model="box3Color">
          <option value="red">Red</option>
          <option value="green">Green</option>
          <option value="blue">Blue</option>
       </select>
      </div>
  </div>
</template>
<script>
import Box from "./Box"
export default {
    components:{
        Box
    },
    data:function(){
        return{
           'box1Color':'',
           'box2Color':'',
           'box3Color':'',
        }
    },
    methods:{
        resetBox1:function(){
            this.box1Color='white'
        },
        resetBox2:function(){
            this.box2Color='white'
        },
        resetBox3:function(){
            this.box3Color='white'
        }
    }
    
}
</script>
<style scoped>
   .row{
       display:flex;
       justify-content:center;
   }
</style>