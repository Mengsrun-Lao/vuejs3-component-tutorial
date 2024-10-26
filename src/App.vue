<template>
 
  <NameList v-slot:default="slotProps">
    {{ slotProps.firstName }} && {{ slotProps.lastName }}
  </NameList>

  <NameList v-slot:default="slotProps">
    {{ slotProps.lastName }} && {{ slotProps.firstName }}
  </NameList>

  <NameList v-slot:default="slotProps">
    {{ slotProps.firstName }} && {{ slotProps.firstName }}
  </NameList>


</template>

<script>
import NameList from './components/NameList.vue';



export default {
  name: 'App',
  components: {
    NameList,
  },
  data(){
    return {
      
    }
  },
  methods:{}
}
</script>



<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>


