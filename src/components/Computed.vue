<template>
    <div>

        <input type="text" name="" id="" placeholder="first-name" v-model="fname">
        <input type="text" name="" id="" placeholder="last-name" v-model="lname">
        <h2>Option API full Name = {{ fullName }}</h2>

        <input type="text" name="" id="" placeholder="Ref_first-name" v-model="refFistName">
        <input type="text" name="" id="" placeholder="Ref_last-name" v-model="refLastName">
        <h2>Option API full Name = {{ refFullName }}</h2>

        <input type="text" name="" id="" placeholder="Reactive_first-name" v-model="recFirstName">
        <input type="text" name="" id="" placeholder="Reactive_last-name" v-model="recLastName">
        <h2>Option API full Name = {{ reactFullName }}</h2>



    </div>
</template>

<script>
import { computed, reactive, ref, toRefs } from 'vue';

    export default {
        name:'computed-component',
        setup(){

            // Using the ref method with the compoisition api 
            const refFistName = ref('')
            const refLastName = ref('')
            const refFullName = computed(function(){
                return `${refFistName.value} ${refLastName.value}`;
            })

            // using the Reactive method with composition api 
            const reactObject = reactive({
                recFirstName : '',
                recLastName  : '',
            });

            const reactFullName = computed(function(){
                return `${reactObject.recFirstName} ${reactObject.recLastName}`;
            })
            
            return {
                refFistName,refLastName,refFullName,
                ...toRefs(reactObject), reactFullName,
            }
        },
        data(){
            return{
                fname:'',
                lname:''
            }
        },
        computed:{
            fullName(){
                return `${this.fname} ${this.lname}`;
            },
        }
    }
</script>

<style scoped>

</style>