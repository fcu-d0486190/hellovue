<template>
  <div id="app">
    <div class="test">
        <h1> {{title}}</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      title: 'h1'
    }
  }
}
</script>

<style>
  .test{
    color: red;
  }
</style>
