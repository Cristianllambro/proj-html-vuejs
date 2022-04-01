<template>
  <div id="app">
    <HeaderContent />
    <UnderHeader />
    <ServiceContent />
    <ToolContent />
    <SquareCream />
    <ReviewContent />
    <BlogContent />
  </div>
</template>

<script>
import HeaderContent from './components/HeaderContent'
import UnderHeader from './components/UnderHeader'
import ServiceContent from './components/ServiceContent.vue'
import ToolContent from './components/ToolContent.vue'
import SquareCream from './components/SquareCream.vue'
import ReviewContent from './components/ReviewContent.vue'
import BlogContent from './components/BlogContent.vue'

export default {
  name: 'App',
  components: {
    HeaderContent,
    UnderHeader,
    ServiceContent,
    ToolContent,
    SquareCream,
    ReviewContent,
    BlogContent,
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
h1, h2, h3{
  font-family: 'Abril Fatface', cursive;
}
</style>
