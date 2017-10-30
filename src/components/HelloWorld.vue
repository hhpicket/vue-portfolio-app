<template lang="pug">
.hello
  h1 {{ msg }}
  h2 {{employee}}
  h2 {{boundStuff}}
  textarea(type="text" v-model.lazy="query")
  h2 {{query}}
  .div
    button.btn.btn-primary(v-on:click="runThisMethod()") Click me To Go To The Other Page
    router-link(to="/About") Go to About
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Look, I made a view JS App',
      employee: 'Hunter Pickett',
      boundStuff: 'More bound stuff',
      query: ''
    }
  },
  methods:
  {
    runThisMethod:function(){
      console.log("hello, you pushed the button");
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
  color: $mike_blue

ul
  list-style-type: none
  padding: 0
  color: $mike_blue

li
  display: inline-block
  margin: 0 10px

a
  color: #42b983
</style>
