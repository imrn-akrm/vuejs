<template>
    <hr>
    <h1>For Loop</h1>
    <h2>Component Name :: {{ componentName }}</h2>
    <ul>
        <li v-for="item in technology" :key="item">{{ item }}</li>
    </ul>
    <br>
    <br>
    <ul>
        <li v-for="item in user" :key="item">
            Name is :: {{ item.name }} and Email is {{ item.email }}

        </li>
    </ul>
    <hr>
</template>
<script>
    export default{
        name:'ForLoop',
        data(){
            return{
                componentName: 'forLoop',
                technology:['java','php','node','html'],
                user:[
                    {name:'name1',email:'email1@email.com'},
                    {name:'name2',email:'email2@email.com'},
                    {name:'name3',email:'email3@email.com'}
                ]
            }
        }
    }
</script>
