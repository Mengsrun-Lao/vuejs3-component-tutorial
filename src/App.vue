<template>

  <ClickCounter/>
  <Hovercounter/>


</template>

<script>
import ClickCounter from './components/ClickCounter.vue';
import Hovercounter from './components/Hovercounter.vue';

 



 
export default {
  name: 'App',
  components: {
    ClickCounter,
    Hovercounter
 
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


