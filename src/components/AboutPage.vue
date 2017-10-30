<template lang="pug">
.about
  h1 {{msg}}
  router-link(to="/") Go Back
</template>

<script>
export default {
  name: 'AboutPage',
  data () {
    return {
      msg: "You've found the second page, wow"
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import "../sass/global.sass"

h1, h2
  font-weight: normal
  text-align: center
  color: $vue_green

ul
  list-style-type: none
  padding: 0

li
  display: inline-block
  margin: 0 10px

a
  color: #42b983
</style>
