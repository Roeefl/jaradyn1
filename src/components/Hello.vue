<template>
  <div class="hello">
    <hr/>
    <div class="form-group">
      <h1>I am the Hello component</h1>
      <h2>{{formData.name}}</h2>
      <input type="text" class="form-control" v-model="formData.value" :name="formData.name">
    </div>
    <hr/>
  </div>
</template>

<script>
  export default {
    name: 'hello',
    props: ['formData'],
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1, h2 {
    font-weight: normal;
    color: red;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>

