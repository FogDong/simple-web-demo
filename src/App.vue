<template>
  <div v-bind:class="{ color: v==='v2.0.0' }">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your KubeVela Demo" v-bind:version="v"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data(){
    return {
      v: 'v2.0.0',
    }
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
  margin-top: 60px;
}
.color {
  background: #005AA7;  /* fallback for old browsers */
  background: -webkit-linear-gradient(to right, #FFFDE4, #005AA7);  /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(to right, #FFFDE4, #005AA7); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  text-align: center;
  padding: 50px 0;
  margin: 0;
}
</style>
