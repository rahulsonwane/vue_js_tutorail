<template>
    <h1> Ref Used for get DOM value Get or Post</h1>
    <input type="text" ref="input" id="input">
    <button v-on:click="getData"  > Get Ref Data</button>
</template>


<script>
export default{
    name:"RefDom",
    methods:{
        getData(){
            this.$refs.input.focus()
            let val = this.$refs.input.value
            console.warn(val)
        }
    }
}
</script>