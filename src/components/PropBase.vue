<template>
<h1> Base of Props vue components student and teachers data</h1>
<h2>{{ childUser}}</h2>
<PropCom :name="name" :getData="getDataName" />
<TeaCher :name="name2" />
</template>

<script>
import PropCom from './PropCom.vue';
import TeaCher from './TeaCher.vue';

export default {
    name: "PropBase",
    data() {
        return {
            name: "Rahul",
            name2: "Sonwane",
            childUser: " "
        }
    },
    components: {
        PropCom,
        TeaCher
    },
    methods: {
        getDataName(name1) {
            this.childUser=name1
        }
    }
}
</script>
