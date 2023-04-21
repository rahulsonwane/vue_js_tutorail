<template>
<h1> Welcome to Two Way Binding </h1>
<input type="text" v-model="count">
<h3> {{ count }}</h3>
</template>


<script>
export default {
    name : 'TwoWayBind',
    data(){
        return {
            count : 10
        }
    }
}
</script>

<style>

</style>