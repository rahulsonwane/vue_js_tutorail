<template>
<h1> Wecome to dynamic components</h1>
<button @click="club='MakeForm'"> MakeForm</button>
<button @click="club='FormModifier'"> FormModifiers</button>
<component :is="club" />

</template>

<script>
import FormModifier from './FormModifier.vue';
import MakeForm from './MakeForm.vue';

export default {
    name: "DnyCom",
    components: {   
        MakeForm,
        FormModifier
    },
    data(){
        return{
            club:'MakeForm'
        }
    }
}
</script>
