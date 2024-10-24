<template>
  <Greet name="Mengsrun-Lao"  heroName="Bun-Meng && Sok-Ny"/>
  <Greet name="Mengsrean-Lao" heroName="Bun-Meng && Sok-Ny"/>
  <Greet name="Mengheang-Lao" heroName="Bun-Meng && Sok-Ny"/>
  <Greet name="Mehghong-Lao"  heroName="Bun-Meng && Sok-Ny"/>
  <Greet :name="name"     :heroName="channel"/>

</template>

<script>
import Greet from './components/Greet.vue';
 

export default {
  name: 'App',
  components: {
    Greet,
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


