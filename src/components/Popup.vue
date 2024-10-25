<template>
    <div>
        <h2>this is the pop-up component</h2>
        <Button @click="$emit('close','THis is the string that passed from child component')">Close button</Button>

    </div>
</template>

<script>
    export default {
        name:'popup-component',
        emits:['close']
    }
</script>

<style scoped>

</style>