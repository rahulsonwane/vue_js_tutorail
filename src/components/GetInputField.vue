<template>
    <h1> Welcome to Two Way Binding </h1>
    <input type="text" placeholder="Enter an Email" v-model="email">
    <br> <br>
    <input type="password" placeholder="Enter a pass" v-model="pass">
    <br> <br>
    <button v-on:click="getData()"> Get Values </button>

    </template>
    
    
    <script>
    export default {
        name : 'GetInputField',
        data(){
            return {
                email : null,
                pass : null
            }
            
        },
        methods:{
            getData(){
                console.warn('Vaues', this.email, this.pass)
            
            }
        }
    }
    </script>
    
    <style>
    
    </style>