<template>
    <h1> Welcome to BeforeUnmounter </h1>
    <button v-on:click="show =!show"> Toggle</button>
    <UnMount v-if="show"/>
</template>

<script>
import UnMount from './UnMount.vue';
export default{
    name:"BeforUnMount",
    data(){
        return{
            show:true
        }
    },
    components:{
        UnMount
    }
}
</script>