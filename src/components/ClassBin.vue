<template>
<h1 :class="applyStyle"> Welcome to Class Binging</h1>
<h2> Css Binding </h2>
<button v-on:click="colorfull=!colorfull"> Click Me</button>
</template>

<script>
export default {
    name: "ClassBin",
    data() {
        return {
            colorfull: false
        }
    },
    computed: {
        applyStyle() {
            return {
                green:this.colorfull,
                err: true,
                other: true

            }
        }
    }
}
</script>

<style>
h2 {
    color: red;
}

.green {
    background-color: green;
    width: 200px;
    padding: 10px;
}

.err {
    color: blue;

}

.other {
    font-size: 50px;
}
</style>
