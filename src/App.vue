<template>


  <button @click="activeTab='TabA'">Tab A</button>
  <button @click="activeTab='TabB'">Tab B</button>
  <button @click="activeTab='TabC'">TaB C</button>

  <keep-alive>
    <component :is="activeTab"/>
  </keep-alive>


</template>

<script>
import TabA from './components/TabA.vue';
import TabB from './components/TabB.vue';
import TabC from './components/TabC.vue';



 
export default {
  name: 'App',
  components: {
    TabA,
    TabB,
    TabC
  },
  data(){
    return {
      value:' ',
      activeTab: 'TabA'
    }
  },
  methods:{
    setValue(component){
      this.value = component ;
    },
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


