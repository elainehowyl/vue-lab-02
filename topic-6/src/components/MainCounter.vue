// Create a MainCounter.vue that has two counters. 
// For each counter, create two buttons - one button to increase the number in the counter, 
// and the other button to decrease. 
// (So you should have four buttons).

// When the user clicks on the counter itself, reset its count to 0 by emitting events.

<template>
    <div>
        <h1>Counter</h1>
        <div class="counter-container">
        <CounterDisplay v-bind:number="counter1Number" v-on:resetNumber="resetCounter1"></CounterDisplay>
        <CounterDisplay v-bind:number="counter2Number" v-on:resetNumber="resetCounter2"></CounterDisplay>
        </div>
    </div>
</template>
<script>
import CounterDisplay from "./CounterDisplay"
export default {
    components:{
        CounterDisplay
    },
    data:function(){
        return{
            'counter1Number':0,
            'counter2Number':0
        }
    },
    methods:{
        resetCounter1:function(){
            this.counter1Number=0;
        },
        resetCounter2:function(){
            this.counter2Number=0;
        }
    }
}
</script>
<style scoped>
.counter-container{
    display:flex;
    flex-direction:row;
    justify-content:center;
}
</style>
