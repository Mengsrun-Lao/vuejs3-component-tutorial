<template>
    <div>
        <h2>this is the pop-up component</h2>
        <input type="text" v-model="name"/>
        <Button @click="$emit('close',name)">Close button</Button>

    </div>
</template>

<script>
    export default {
        name:'popup-component',
        // emits:['close'],
        emits:{
            close: (name)=>{
                if(!name){
                    return false
                }
                else{
                    return true
                }
            }
        },
        data(){
            return {
                name: ''
            }
        },

    }
</script>

<style scoped>

</style>