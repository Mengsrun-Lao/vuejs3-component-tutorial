<template>
    <div>
        <h2>Article Component</h2>
        <h3>{{ title }}</h3>
        <h3 v-bind="$attrs">The Number value {{ like }}</h3>
        <h3>The Bolean value {{ isPublised ? 'yes': 'No' }}</h3>
    </div>
</template>

<script>
    export default {
        name:'ArticleComponent',
        props:{
            title:{
                type: String,
                require: true,
                default: 'Article default value'
            },
            like: Number,
            isPublised: Boolean,
        },
        inheritAttrs:false
    }
</script>

<style scoped>

</style>