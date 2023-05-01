<template>
<h1> Using non-props data in non-prop-base components </h1>
<div  >
    <h3>Rahul </h3>
    <h3 >Vishal</h3>
    <h3  v-bind="$attrs">Sandeep</h3>
    <h3> {{ data }}</h3>

</div>
</template>

<script>
export default {
    name: "NonProp",
    props: {
        data: String
    }
}
</script>
