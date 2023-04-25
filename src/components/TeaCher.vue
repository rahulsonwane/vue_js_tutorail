<template>
    <h1>Welcome to Teachers name is: {{ name }}</h1>
</template>

<script>
export default{
    name:"TeaCher",
    props:{
        name:String
    }
}
</script>