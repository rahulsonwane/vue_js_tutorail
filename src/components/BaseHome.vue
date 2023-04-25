<template>
<h1> Welcome to Base page</h1>
<ul>
    <li v-for="item in users" :key="item">
        <ReuseCompo :data="item" :getData="getData"/>
        
    </li>
</ul>


</template>

<script>
import ReuseCompo from './ReuseCompo.vue';

export default {
    name: "BaseHome",
    components: {
        ReuseCompo
        
    },
    methods:{
        getData(name, email){
            alert(name, email)
        }
    },
    data() {
        return {
            users: [{
                name: 'pritam',
                email: 'pritam@gmail.com'   
            },
            {
                name: 'rahul',
                email: 'rahul@gmail.com'   
            },
            {
                name: 'vishal',
                email: 'vishal@gmail.com'   
            },
            {
                name: 'sandeep',
                email: 'sandeep@gmail.com'   
            }
        ]

        }
    }
}
</script>
