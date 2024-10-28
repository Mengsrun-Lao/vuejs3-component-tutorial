<template>
    <div>
        <h3 :style="{color:'blue', background:'red'}">This is the Tab C is working</h3>
        <input type="text" v-model="value">
    </div>
</template>

<script>
    export default {
        name:'tabC-component',
        value:''
    }
</script>

<style scoped>

</style>