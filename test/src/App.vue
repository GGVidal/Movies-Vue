<template>
  <div id="app">
    <div class="sidebar">

    </div>
    <HelloWorld/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style>
  .sidebar {
    height: 25px;
    background: rgb(2, 136,209);
  }
</style>
