<template>
    <hr>
    <h1>For Each Loop</h1>
    <h2>Component Name :: {{ componentName }}</h2>
    <ul>
        <!-- Loop Iterations -->
    </ul>
    <br>
    <br>
    <ul>
        <!-- For each loop iterations -->
    </ul>
    <hr>
</template>
<script>
    export default{
        name:'ForEachLoop',
        data(){
            return{
                componentName: 'forEachLoop',
                technology:['java','php','node','html','vue','angular','sencha'],
                user:[
                    {name:'imran',email:'imran@imran.com'},
                    {name:'ahad',email:'ahad@ahad.com'},
                    {name:'ahmad',email:'ahmad@ahmad.com'}
                ]
            }
        }
    }
</script>
<style>
* {
  background-color:#ccc;
  color:#000;
}
a {
  color:#000;
  text-decoration:none;
}  
  h1{
    color:blue;
  }
  h2{
    color:green;
  }
  h3{
    color:maroon;
  }
  .warning{
    color:red;
  }
  #title{
    font-size:14px;
    font-weight:bolder;
  }
</style> 
