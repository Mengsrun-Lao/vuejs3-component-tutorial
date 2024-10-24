<template>
 
  <Article id="my-attribute" title="titile is string type" :like="40" :isPublised="true" />

</template>

<script>

import Article from './components/Article.vue';

export default {
  name: 'App',
  components: {
    Article,
  },
  data(){
    return{
      name:'Mengxing',
      channel:'Ting-Ting'
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
</style>


