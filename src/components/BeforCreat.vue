<template>
    <h1> Welcome before and created using {{ name }}</h1>
</template>

<script>
export default{
    name:"BeforCreat",
    data(){
        console.warn("createdd.")
        return{
            name:"Rahul"
        }
    },
    beforeCreate(){
        alert("Before Create");
    },
    created(){
        this.name="Sonwane"
        alert("Created")
    }
}
</script>