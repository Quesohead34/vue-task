// this is the button component that adds new tasks to todo list //

<template>
    <button @click="onClick()" :style="{background: color}" class="btn">Add Task</button>
</template>

// this is the logic for adding btn functionality & props for the button //
// **note** props will allow btn to inherit color from called component in main component header file //
<script>
    export default {
        name: 'Button',
        props: {
            text: String,
            color: String
        },
        methods: {
            onClick() {
                console.log('click')
            }
        }
        }
</script>