<template lang="pug">
  .div#app
    img(src="./assets/logo.png")
    router-view
</template>

<script>
export default {
  name: 'app'
}
</script>

<style lang="sass">
#app
  div
    text-align: center
  img
    display: block
    margin: 0 auto
</style>
