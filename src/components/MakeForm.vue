<template>
<h1> Welcome to Vue Js Form </h1>

<p>
    {{ form }}
</p>
<form >
    <div class="email">
        <label> Email : </label>
        <input type="email" name="email" placeholder="Enter Email" v-model="form.email">
    </div>

    <div class="pass">
        <label> Pass : </label>
        <input type="password" name="password" placeholder="Enter password" v-model="form.password" >
    </div>

    <button  v-on:click="login" type="button"> Login </button>
</form>
</template>

<script>
export default {
    name: "MakeForm",
    data(){
        return{
            form:{
                email:" ",
                password:" "
            }
        }
    },
    methods:{
        login(){
            console.log("login data", this.form)
        }
    }
}
</script>

<style>
.email {
    margin-bottom: 10px;
}

button {
    margin-top: 10px;
}
</style>
