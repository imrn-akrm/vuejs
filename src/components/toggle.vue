<template>
    <hr>
    <h1>toggle</h1>
    <h2>component :: {{ componentName }}</h2>
    <h2 v-if="show">True</h2>
    <h2 v-else>False</h2>
    <button v-on:click="show=!show">Toggle</button>

    <hr>
</template>
<script>
    export default{
        name:'toggleComponent',
        data(){
            return{
                compoentName:'Toggle',
                show:true
            }
        }
    }
</script>
