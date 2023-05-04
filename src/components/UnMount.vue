<template>
    <h1 ref="user"> Welcome to Unmounted </h1>
</template>

<script>
export default{
    name:"UnMount",
    beforeUnmount(){
        console.log("BeforUnmount", this.$refs['user'])
    },
    unmounted(){
        console.log("Unmounted", this.$refs['user'])
    }
}
</script>