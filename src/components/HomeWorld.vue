<template>
  <h1> Welcome to Home and ready to work</h1>
  <h3> Email {{ email }}</h3>
  

  <button v-on:click="getData()"> ADD</button>
  <button v-on:click="getData1()"> Sub</button>

  <h2> {{ count }}</h2>

</template>

<script>
export default {
  name: 'HomeWorld',
  data() {
    return {
      count : 0
      
    }
  },
  methods: {
    getData() {
      this.count = this.count+1
    },
    getData1(){
      this.count = this.count -1
    }
    
  }
  
}



</script>


<style scoped>
h1 {
  color: red;
}

h5 {
  color: rgb(71, 30, 37);
  font-size: large;
}
</style>