<template>
  <NavComponent/>
  <CardComponents/>
</template>

<script>
import NavComponent from './components/NavComponent.vue'
import CardComponents from './components/CardComponents.vue'

export default {
  name: 'App',
  components: {
    NavComponent,
    CardComponents
  }
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
</style>
