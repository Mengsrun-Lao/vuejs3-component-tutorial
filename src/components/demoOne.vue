<template>
    <div>
        <h3>{{ name }}</h3>
    </div>
</template>

<script>
import { ref } from 'vue';

    export default {
        name:'demoOne-component',
        setup(){
            const name = ref('demo-One')


            setTimeout(()=>{
                name.value = 'change to something else in 200$',
                console.log(name)
            },2000)

            return {
                name,
            }
        },
        
    }
</script>

<style scoped>

</style>