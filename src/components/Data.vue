<template>
    <div>
        <h3>Option API = {{ o_firstName }}</h3> <br>

        <h3>Composition API = {{ c_firstName }}</h3>
        <h3 :style="{color:'red'}">Composition API = {{ newValue }}</h3>

    </div>
</template>

<script>
import { ref } from 'vue';

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

            return {
                c_firstName,
                newValue
            }
        }
        
    }
</script>

<style scoped>

</style>