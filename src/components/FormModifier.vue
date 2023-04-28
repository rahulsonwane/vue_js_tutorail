<template>
    <h1> Form Modifiers </h1>
    <input type="text" v-model.lazy="data">  
    <!-- <input type="text" v-model.trim="data"> -->
 <!-- used for input value print after the enter  -->
 <br/> <br/>
    <input type="number" v-model.number="data">
    only number are print 

    <h2>  Name is: {{ data }}</h2>
    <h3> Type of input : {{ typeof(data) }}</h3>
</template>


<script>
export default{
    name:"FormModifier",
    data(){
        return{
            data:''
        }
    }
}
</script>