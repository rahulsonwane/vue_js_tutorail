<template>

<div class="user">
    <h1> {{ data.name }}</h1>
    <h1> {{ data.email }}</h1>
    <button v-on:click="getData(data.name,data.email)"> Alert Name</button>
</div>

</template>

<script>
export default {
    name: 'ReuseCompo',
    props:{
        data:Object,
        getData:Function
    },
    
    
}
</script>

<style>
.user{
    background-color: navy;
    color: white;
    border: 1px solid;
    margin-bottom: 3px;
}
</style>
