<template>
<Nav/>

   <router-view :data="data"></router-view>

</template>

<script>

import Nav from './Nav';

import data from './data'



export default {
  name: 'App',
  data(){
  return {
  data: data
  }
  },

  components: {
    Nav,
        data,

  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

}
</style>
