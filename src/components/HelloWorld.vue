<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      For more information about KubeVela<br>
      check out the
      <a href="https://kubevela.io/" target="_blank" rel="noopener">KubeVela Documentation</a>.
    </p>
    <h3>Current Demo Version</h3>
    <ul>
      <b>{{ version }}</b>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    version: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
  color: #5b98df;
}
</style>
