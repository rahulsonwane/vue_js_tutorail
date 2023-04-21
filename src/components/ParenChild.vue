<template>
    <h1> Data Tarnsfer parent to child Helloword.vue</h1>
    <h3> {{ name }}</h3>
    <h4> {{ user }}</h4>
    <button v-on:click="getData()"> Call Function </button>
</template>

<script>
export default{
    name: 'ParenChild',
    props :{
        name:String,
        user:Object,
        getData: Function
    }
    
}
</script>