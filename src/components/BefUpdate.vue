<template>
    <h1> Welcome used of BeforeUpdate and updated </h1>
    <h2 ref="count"> {{ counter }}</h2>
    <button v-on:click="counter=counter + 1"> Update Count</button>
</template>

<script>
export default{
    name:"BefUpdate",
    data(){
        return{
            counter:0
        }
    },
    beforeUpdate(){
         console.log("beforeUpdate", this.$refs['count'].textContent)
    },
    updated(){
        console.log("Updated", this.$refs['count'].textContent)

    }
}
</script>