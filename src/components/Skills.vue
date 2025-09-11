<template>
  <div class="hello">
    <div class="holder">
      <ul>
        <li v-for="(data, index) in skills" :key='index'>{{ index }}. {{ data.skill }}</li>
      </ul>

      <p v-if="skills.length >= 1">You have more than 1 skills</p>
      <p v-else>You have less than 1 skill</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SkillsList',
  data() {
    return {
      skills: [
        { "skill": "Vue.js" }, 
        { "skill": "Frontend Developer" } 
      ]
    }
  },
  mounted() {
    console.log("Mounted hook triggered ✅")
    console.log("VUE_APP_TITLE:", process.env.VUE_APP_TITLE)
    console.log("VUE_APP_API_URL:", process.env.VUE_APP_API_URL)
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
  color: #42b983;
}
</style>
