<template>
    <h1 v-if="show">Welcome to If  condition</h1>
    <h1 v-else>Welcome to  Else condition</h1>

    <button v-on:click="show =! show" > Toggle</button>

</template>


<script>
export default {
    name: 'IfElse',
    data(){
        return{
            show: true
        }
    }
}
</script>

<style>

</style>