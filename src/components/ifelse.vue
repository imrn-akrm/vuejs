<template>
    <hr>
    <h1>if else</h1>
    <h2>Compoent Name :: {{ componentName }}</h2>
    <h3>Condition is returning :: <span v-if="show">True</span><span v-else>False</span></h3>
    <hr>
</template>
<script>
    export default{
        name: 'IfElseComponent',
        data(){
            return{
                componentName: 'IfElseComponent',
                show:false
            }
        }
    }
</script>
<style>

</style>
