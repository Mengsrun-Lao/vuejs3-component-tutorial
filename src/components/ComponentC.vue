<template>
    <div>
        <h2>Component C</h2>
        <ComponentE />
    </div>
</template>

<script>
import ComponentE from './ComponentE.vue';
    export default {
        components:{
            ComponentE,
        },
        data(){
            return {
                dynamicName:'Meng-Meng',
            }
        },
        provide(){
            return {
                username: this.dynamicName, 
            }
        }

        // This called the object, if we want to pass the value as dynamic . we cannot use object, if object the child component wil reference to the old value
        // that's why the main reason , you have to use as the function instead. this makes sense for this as well . 
        // provide:{
        //     username: 'Mengsrun'
        // }
        
    }
</script>
 