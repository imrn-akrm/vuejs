<template>
  <div class="hello-imran">
    <h1>{{ msg }}</h1>
    
  </div>
</template>

<script>
export default {
  name: 'HelloImran',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
</style>
