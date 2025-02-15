<template>
    <hr>
    <h1>Two Way Binding</h1>
    <h2>{{ componentName  }}</h2>
    <input type="text" v-model="count">
    <h1>{{ count }}</h1>
    <hr>
</template>
<script>
    export default{
        name: 'TwoWayBinding',
        data(){
            return{
                componentName: "Component Name: Two Way Binding",
                count:555
            }
        }
    }
</script>
<style scoped>
    h1{
        color:brown;
        font-size: small;
        font-weight:bold;
    }
    h2{
        color:maroon;
        font-size: smaller;
    }
</style>
