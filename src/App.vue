<template>

  <h2>using for  Reactivity </h2>
  <DemoOne/> <br><br>


  <h2>Using with toRef</h2>
  <DemoTwo/>

  

</template>

<script>
import DemoOne from './components/demoOne.vue';
import DemoTwo from './components/demoTwo.vue';

 
 



 
export default {
  name: 'App',
  components: {
    DemoOne,
    DemoTwo
 
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


