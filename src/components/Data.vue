<template>
    <div>
        <h3>Option API = {{ o_firstName }}</h3> <br>

        <h3>Composition API = {{ c_firstName }}</h3>
        <h3 :style="{color:'red'}">Composition API = {{ newValue }}</h3> 

        <h3>Using Reactive to replace Data = {{ user.userName }} &&  {{ user.email }}</h3>

    </div>
</template>

<script>
import { reactive, ref } from 'vue';

    export default {
        name:'data-coponent',
        data(){
            return{
                o_firstName:'Option api'
            }
        },

        // Using with Composition API 
        setup(){
            const c_firstName = ref('Composition API')
            // set new value for data with using composition api
            const newValue = `update for ${c_firstName.value}`;

            // using the reactive method
            const user = reactive({
                userName:'John',
                email:'jonh@gmail.com',
            })

            return {
                c_firstName,
                newValue,

                user
            }
        }
        
    }
</script>

<style scoped>

</style>