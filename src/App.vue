<template>
  <div id="app">
    <login/>
    <roles/>
  </div>
</template>
<script>
import login from './components/login.vue'
import roles from './components/roles.vue'
export default {
  name:"app",
  components: {
    login,
    roles
  },
  data() {
    return {
      
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
}

</style>
