<template>
    <div>
        <h3 @mouseover="incrementCount" :style="{color:'blue'}">hover to count value => Number {{ count }}</h3>
    </div>
</template>

<script>
import counter from '@/mixins/counter';

    export default {
        name:'hoverCounter-component',
        mixins:[counter]
    }
</script>

<style scoped>

</style>