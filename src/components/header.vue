<template>
    <header>
        <h1>{{ title }}</h1>
        <Button text="Add Task" color="black" />
    </header>
</template>

<script>
import Button from "./Button.vue";
export default {
    name: "Header",
    props: {
        title: {
            type: String,
            required: true,
        },
    },
    components: {
        Button,
    },
};
</script>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>
