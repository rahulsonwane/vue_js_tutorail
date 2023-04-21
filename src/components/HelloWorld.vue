<template>
<div class="hello">
    <h1>{{ msg }}</h1>
</div>
<ParenChild name="Rahul" :user="user" :getData="getData"/>
</template>

<script>
import ParenChild from './ParenChild.vue';

export default {
    name: "HelloWorld",
    props: {
        msg: String
    },
    components: {
        ParenChild
    },
    data() {
        return {
            user: {
                name: 'Pritam',
                email: 'pritam@gmail.com'
            }
        }
    },
    methods: {
      getData(){
      console.warn("parent function call"),
      alert("Hello ")
      }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
h3 {
    margin: 40px 0 0;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    display: inline-block;
    margin: 0 10px;
}

a {
    color: #42b983;
}
</style>
