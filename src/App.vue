<template>
  <div id="app">
    <HeaderContent />
  </div>
</template>

<script>
import HeaderContent from './components/HeaderContent'

export default {
  name: 'App',
  components: {
    HeaderContent
  }
}
</script>

<style lang="scss">
#app {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
