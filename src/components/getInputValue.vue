<template>
    <hr>
    <h1>
        Get Input value
    </h1>
    <h2>
        {{ componentName }}
    </h2>
    <input type="text" v-model="name" class="inputField" placeholder="enter user name">
    <input type="password" v-model="password" class="inputField" placeholder="enter password">
    <button type="button" v-on:click="getUserData()">Login</button>
    <hr>
</template>
<script>
    export default{
        name: 'GetInputvalue',
        data(){
            return{
                componentName: 'Component Name:: GetInputValue',
                name:null,
                password:null
            }
        },
        methods:{
            getUserData(){
                console.warn(this.name, this.password)
            }
        }
    }
</script>
<style>
    h1{
        color:steelblue;
        font-size:12px;
        font-weight:bold;
    }
    h2{
        color:teal;
        font-size:12px;
    }
    .inputField{
        margin-top:15px;
        margin-bottom:15px;
    }

</style>
