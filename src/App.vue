<template>

  <button @click="setValue('componentA')">Button A</button>
  <button @click="setValue('componentB')">Button B</button>
  <button @click="setValue('componentC')">Button C</button> 

  <Tab :class="styleSlot"> 
    {{value}}
  </Tab>



</template>

<script>
import Tab from './components/Tabs.vue';

 
export default {
  name: 'App',
  components: {
      Tab  
  },
  data(){
    return {
      value:' '
    }
  },
  methods:{
    setValue(component){
      this.value = component ;
    },
  },
  computed:{
    styleSlot(){
      return {
        'style-A': this.value === 'componentA',
        'style-B': this.value === 'componentB',
        'style-C': this.value === 'componentC',
      }
    }
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


