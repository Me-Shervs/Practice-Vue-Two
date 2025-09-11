<template>
  <div id="app">
    <SkillsList/>
  </div>
</template>

<script>
import SkillsList from './components/Skills.vue'

export default {
  name: 'App',
  components: {
    SkillsList
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
