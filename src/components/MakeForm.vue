<template>
<h1> Welcome to Vue Js Form </h1>

<p v-for="item in form" :key="item">
    <ul>
       {{ item}}
       
    </ul>
    
</p>
<form>
    <div class="email">
        <label> Email : </label>
        <input type="email" name="email" placeholder="Enter Email" v-model="form.email">
    </div>

    <div class="pass">
        <label> Pass : </label>
        <input type="password" name="password" placeholder="Enter password" v-model="form.password">
    </div>
    <br /> <br />
    <div class="select">
        <select v-model="form.country">
            <option>India</option>
            <option>Japan</option>
            <option>Finland</option>
        </select>
    </div>

    <br /> <br />
    <div class="technology">
        <h3> Technology </h3>
        <label> Python : </label>
        <input type="checkbox" value="Python" v-model="form.technology">
        <br /> <br />
        <label> Django : </label>
        <input type="checkbox" value="Django" v-model="form.technology">
    </div>

    <div class="gender">
        <h3> Gender </h3>
        <label> Male </label>
        <input type="radio" value="male" v-model="form.Gender">
        <br /> <br />
        <label> Female </label>
        <input type="radio" value="female" v-model="form.Gender">
    </div>

    <button v-on:click="login" type="button"> Login </button>
</form>
</template>

<script>
export default {
    name: "MakeForm",
    data() {
        return {
            form: {
                email: " ",
                password: " ",
                country: " ",
                technology: [],
                Gender: " "

            }
        }
    },
    methods: {
        login() {
            console.log("login data", this.form)
        }
    }
}
</script>

<style>
.email {
    margin-bottom: 10px;
    margin: 10px;
}

button {
    margin-top: 10px;
}

.country {
    margin-top: 10px;
}

form {
    margin: auto;
    width: 300px;
    padding: initial;
    border: 1px solid black;
    background-color: pink;
}
</style>
