<template>
<div class="card">
    <ChildSlot>
        <template v-slot:header>
            <h1>Welcome to slot topic1</h1>
        </template>
        <template v-slot:info>
            <h1>Rahul Sonwane</h1>
        </template>
        <template v-slot:footer>
            <button> Buy Now</button>
        </template>

    </ChildSlot>
    <ChildSlot>
        <template v-slot:header>
            <h1>Welcome to slot topic1</h1>
        </template>
        <template v-slot:info>
            <h1>Rahul Sonwane</h1>
        </template>
        <template v-slot:footer>
            <button> Click Me </button>
        </template>

    </ChildSlot>
    <ChildSlot>

    </ChildSlot>
</div>
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
