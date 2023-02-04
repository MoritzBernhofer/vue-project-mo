<template>
    <button @click="onClick()" :style="{ background: color }" class="btn">
        {{ text }}
    </button>
</template>

<script>
export default {
    name: "Button",
    props: {
        text: {
            type: String,
            required: true,
        },
        color: {
            type: String,
            default: "steelblue",
        },
    },
    methods: {
        onClick() {
            console.log("Hello there");
        },
    },
};
</script>
