<template>
<div class="card">
    <slot name="header">
    </slot>
    <slot name="info"></slot>
    <slot name="footer"></slot>
</div>
</template>

<script>
export default {
    name: "ChildSlot",
    props: {
        data: String
    }

}
</script>

<style>
.card {
    border: 1px black solid;
    width: 500px;
    background: aquamarine;
    height: 200px;
    margin-bottom: 3px;
}
</style>
