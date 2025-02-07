<template>
    <hr>
    <h1>events</h1>
    <h2 v-on:mousemove="onMouseMove()">{{ componentName }}</h2>
    <button v-on:click="test()">click</button>
    <button v-on:click='getClick("Single Clicked")'>Single Click</button>
    <button v-on:dblclick='getClick("Double Clicked")'>Double Click</button>
    <button v-on:click='getIncrement()'>Click to Increment</button>
    <button v-on:click='getDecrement()'>Click to Decrement</button>
    <h2>{{ countwww }}</h2>
    <hr>
</template>
<script>
    export default{
        name: 'EventsComponent',
        data(){
            return {
                componentName: 'Events in VueJs',
                countwww:5
            }
        },
        methods:{
            getIncrement(){
                this.countwww=this.countwww+1
            },
            getDecrement(){
                this.countwww=this.countwww-1
            },
            test(){
                alert("Clicked")
            },
            getClick(a){
                alert(a)
            },
            onMouseMove(){
                console.warn("Mouse Moved on Component name")
            }
        }
    }
</script>
<style scoped>
    h1{
        color: blueviolet;
        font-size: small;
    }
    h2{
        color: chocolate;
        font-size: smaller;
    }
</style>
