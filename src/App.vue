<template>

  <Data/>

</template>

<script>
import Data from './components/Data.vue';

 
 



 
export default {
  name: 'App',
  components: {
    Data
 
  },
  data(){
    return {
    }
  },
  methods:{
  },
  computed:{ 
  }
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

.style-A{
  color: red;
  font-style: italic;
  font-weight: bold;
}
.style-B{
  color: blue;
}
.style-C{
  color: green;
}
 
</style>


