// this is the main app components template containing other components //
<template>
    <header>
        <h1>Task Tracker</h1>
        <Button text= "Add Task" color= "green"/>
    </header>
</template>

// this is the main logic that contains imports of related components & functionality //

<script>

import Button from './Button'

export default {
    name: 'Header',
    props: {
        title: String,
    },
    components: {
        Button
    }
}
</script>

// this is the styling for the main component since scoped it will only apply to this component //


<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}    
</style>