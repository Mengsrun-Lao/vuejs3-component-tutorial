<template>
    <h3 v-for="name in names" :key="name.firstName">
        <slot :firstName="name.firstName" :lastName="name.lastName"></slot>
    </h3>
</template>

<script>
    export default {
        name:'nameList-component',
        data(){
            return {
                names:[
                    {
                        firstName: 'firstName-1111',
                        lastName : 'lastName-1111'
                    },
                    {
                        firstName: 'firstName-2222',
                        lastName : 'lastName-2222'
                    },
                    {
                        firstName: 'firstName-3333',
                        lastName : 'lastName-3333'
                    },
 
                ]
            }
        }
    }
</script>

<style scoped>

</style>