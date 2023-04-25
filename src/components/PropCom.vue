<template>
<h1> Welcome Student name is : {{ name }} </h1>
<button v-on:click="getData(name1)">Send User Name </button>
</template>

<script>
export default {
    name: "PropCom",
    data() {
        return {
            name1: "Parent to Child"
        }
    },
    props: {
        name: String,
        getData: Function
    }

}
</script>
