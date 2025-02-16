<template>
    <hr>
    <h1>Home Component {{ 10+10 }}</h1>
    <h1>Home Component {{ "10+10".length }}</h1>
    <h1>Email is  {{email}}</h1>
    <h1>Mobile is  {{mobile}}</h1>
    <h1>Assign Value during interpolation Acyual value is 0300 but new is now ::  {{ mobile=888 }}</h1>
    <h1>Functoin returned : {{ getname() }}</h1>
    <h1>Method that return static text : {{ getNameStatic() }}</h1>
    <h1>Method that return dynamic text : {{ getNameDynamic("Text Set from Html as parameter") }}</h1>
    <h1>Method that retun Object complete : {{ getDataObject() }}</h1>
    <h1>return only specific value from a methods object : {{ getDataObject().objects_first_value }}</h1>
    <h1>Use of this : {{ this.email }}</h1>
    <h1>Use of this : {{ this }}</h1>
    <hr>
</template>
<script>
    export default{
        name:'HomeComponent',
        data(){
            return{
                email:'admin@admin.com',
                mobile:'0300',
                getname:function(){
                    return "text from function"
                }
            }
        },
        methods:{
            getNameStatic(){
                return "Static Name"
            },
            getNameDynamic(nameComingFromFunctionCall){
                return nameComingFromFunctionCall
            },
            getDataObject(){
                return{
                    objects_first_value: 'oject 1st value',
                    objects_second_value: 'object 2nd value'
                }
            }
        }
    }
</script>
<style scoped>
    h1{
        color:orange;
        font-size: small;
    }
</style>
