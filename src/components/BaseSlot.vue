<template>
<ChildSlot>
    <h1>Welcome to slot topic</h1>
</ChildSlot>
<ChildSlot>
    <h1>Rahul Sonwane</h1>
</ChildSlot>
<ChildSlot> <img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.linkedin.com%2Fcompany%2Fnetserv-llc&psig=AOvVaw2rheOalIzbIgUwu8LER82d&ust=1683204972098000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCODDpKWZ2f4CFQAAAAAdAAAAABAE" > Netserv </ChildSlot>
</template>

<script>
import ChildSlot from './ChildSlot.vue';
export default {
    name: "BaseSlot",
    components: {
        ChildSlot
    }
}
</script>
