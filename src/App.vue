<template>
  <div id="app">
    <hr/>
    <img src="./assets/logo.png">
    <h1>I am the App component</h1>
    <h3>I show the current value in formData.value: {{formData.value}}</h3>
    <hello :formData='formData'></hello>
  </div>
</template>

<script>
import Hello from './components/Hello'

export default {
  name: 'app',
  data () {
    return {
      formData: {
        name: 'Address Form',
        value: 'Area 51'
      }
    }
  },
  components: {
    Hello
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
