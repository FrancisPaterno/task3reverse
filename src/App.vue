<template>
  <div id="app">
     <label for="input-text">Enter text here:</label>
    <input type="text" id="input-text" v-model="text"/>
   
    <Reverse :text="text"/>
  </div>
</template>

<script>
import Reverse from './components/Reverse.vue';
export default {
  name: 'App',
  components: {
    Reverse
  },
  data(){
    return {text:''}
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
