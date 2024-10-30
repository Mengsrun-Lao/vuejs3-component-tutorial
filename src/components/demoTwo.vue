<template>
    <div>
        <h2>First Name : {{ firstName }}</h2>
        <h2>Last Name : {{ lastName }}</h2>
    </div>
</template>

<script>
import { reactive, toRefs } from 'vue';

    export default {
        name:'demoTwo-componet',
        setup(){
            const state = reactive({
                firstName: 'FirstName',
                lastName:' lastName',
            })

            setTimeout(()=>{
                state.firstName = 'firstname using reactive',
                state.lastName  = 'lastname using reactive'
                 
            },2000)

            return {
                ...toRefs(state)
            }
        }
    }
</script>

<style scoped>

</style>