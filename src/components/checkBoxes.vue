<template>
    <hr>
    <h1>Check Boxes</h1>
    <h2>{{ componentName }}</h2>
    <h3>Technology</h3>
    <label for="java">Java</label>
    <input type="checkbox" value="java" name="" id="java" v-model="technology"><br><br>
    <label for="php">PHP</label>
    <input type="checkbox" value="php" name="" id="php" v-model="technology"><br><br>
    <label for="node">Node</label>
    <input type="checkbox" value="node" name="" id="node" v-model="technology"><br><br>

    <h4>Selected Technology: {{ technology }}</h4>

    <br><br>
    <h4>Who i am</h4>
    <label for="student">Student</label>
    <input type="radio" value="student" name="who" v-model="who" id="student"><br><br>
    <label for="developer">developer</label>
    <input type="radio" value="developer" v-model="who" name="who" id="developer"><br><br>
    <h4>I am a :: {{ who }}</h4>
    <hr>
</template>


<script>
    export default{
        name: 'CheckBoxes',
        data(){
            return{
                componentName:'Component Name : Check Boxes',
                technology:[],
                who:null
            }
        }
    }
</script>
<style></style>
