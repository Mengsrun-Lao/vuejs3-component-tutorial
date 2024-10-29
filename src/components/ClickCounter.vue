<template>
    <div>
            <button @click="incrementCount">Increase Number {{ count }}</button>
    </div>
</template>

<script>
import counter from '@/mixins/counter';

    export default {
        name:'clickCounter-component',
        mixins: [counter,]
        
    }
</script>

<style scoped>

</style>