
<template>
    <div class="counter">
        <div class="counter-container">
        <button v-on:click="decrement"> - </button>
        {{this.number}}
        <button v-on:click="increment"> + </button>
        </div>
        <button v-on:click="resetto0">Reset to Zero</button>
    </div>
</template>

<script>
export default {
    props:['number'],
    methods:{
        decrement:function(){
            this.number -= 1
        },
        increment:function(){
            this.number += 1
        },
        resetto0:function(){
            this.$emit('resetNumber');
        }
    }
}
</script>

<style scoped>
.counter {
    width: 250px;
    height: 250px;
    text-align:center;
    border:1px black solid;
}
.counter-container{
    display:flex;
    align-items:flex-end;
    justify-content:center;
}
</style>
