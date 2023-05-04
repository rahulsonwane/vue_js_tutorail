<template>
<h1> Welcome to Before Mount and Mount {{ name }}</h1>
<h2> Learn for vue.js </h2>
</template>

<script>
export default {
    name: "BefMount",
    data() {
        return {
            name: "Pritam"
        }
    },
    beforeMount() {
        console.warn("beforeMount", this.$el)
    },
    mounted() {
        console.warn("Mounted", this.$el)
    }
}
</script>
