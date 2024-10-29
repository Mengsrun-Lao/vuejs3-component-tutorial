<template>
    <div>
        <input type="text" name="" id="" ref="inputRef">
    </div>
</template>

<script>
    export default {
        name:'templateRef-component',
        mounted(){
            this.$refs.inputRef.focus();
        },
    }
</script>

<style scoped>

</style>