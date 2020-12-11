<template>
  <div v-bind:style="{backgroundColor:bgColor}" class="boxes">
        {{content}}
        <br><button v-on:click="reset">Reset</button>
  </div>
</template>
<script>
export default {
    data:function(){
        return{

        }
    },
    props:['bgColor','content'],
    methods:{
        reset:function(){
           this.$emit('reset_backgroundcolor');
        }
    }
}
</script>
<style scoped>
  .boxes{
      height:200px;
      width:200px;
      border:solid;
  }
</style>