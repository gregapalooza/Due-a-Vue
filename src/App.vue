<template>
  <div id="app">
    <Header theTitle="Vue to Due"/>
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
   Header
  }
}
</script>

<style>
  * {
    margin: 0;
    pad: 0;
  }
</style>
