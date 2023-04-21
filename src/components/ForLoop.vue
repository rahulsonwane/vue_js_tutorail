<template>
<h1> Welcome to for loop</h1>
<ul>
    <li v-for="item in technology" :key="item">
        {{ item }}
    </li>
</ul>
<br><br>
<ul>
    <li v-for="item in user" :key="item.email">
        Name is : {{ item.name}} and <br>
        Email is : {{ item.email }}
    </li>
</ul>
</template>

<script>
export default {
    data() {
        return {
            technology: ['HTMl', 'CSS', 'JavaScript', 'Python', 'Django', 'Vue'],
            user: [{
                    name: 'Rahul',
                    email: 'rahul@gmail.com'
                }, {
                    name: 'pritam',
                    email: 'pritam@gmail.com'
                },
                {
                    name: 'vishal',
                    email: 'vishal@gmail.com'
                }

            ]
        }
    }
}
</script>
