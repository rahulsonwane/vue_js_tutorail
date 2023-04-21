<template>
    <h1> Welcome Get Radio and Checkbox values.</h1>
    <h3> Technology </h3>
    <label for="java"> Java</label>
    <input type="checkbox" value="Java" id="java" v-model="technology">

    <label for="python"> Python</label>
    <input type="checkbox" value="Python" id="python" v-model="technology">

    <br><br>
    <h3> Who I am </h3>
    <label for="student"> Student </label>
    <input type="radio" value="student" v-model="who" id="student" name="who">

    <label for="developer"> Developer </label>
    <input type="radio" value="developer" v-model="who" id="developer" name="who">

    <h4> Selected Technology : {{ technology }}</h4> 
    <h4> Who I am  : {{ who }}</h4>    


</template>


<script>
export default{
    name: "CheckRadiBut",
    data(){
        return{
            technology : [],
            who: null
        }
    }
}
    

</script>



<style>

</style>