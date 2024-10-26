<template>

  <h4>App component Text</h4>
  <ChildStyle>
    <h4>Testing the child componen</h4>
  </ChildStyle>

</template>

<script>
import ChildStyle from './components/ChildStyle.vue';



export default {
  name: 'App',
  components: {
      ChildStyle
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
h4 {
  color: red;
}
</style>


