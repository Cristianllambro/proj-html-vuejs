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
@import url('https://fonts.googleapis.com/css2?family=Abril+Fatface&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;500&display=swap');
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
p{
  font-family: 'Roboto', sans-serif;
}
</style>
