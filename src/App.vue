<template>
  <div id="app">
   <!-- HEADER -->
  <Header/>
  <!-- CONTENT -->
  <Content/>
  <!-- MAIN -->
  <Main/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Content from '@/components/Content.vue'
import Main from '@/components/Main.vue'

export default {
  name: 'App',
  components: {
    Header,
    Content, 
    Main,
  }
}
</script>

<style lang="scss">
* { 
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  #app {
    margin: 0 auto;
  font-family: 'Open Sans', sans-serif;
  }
</style>
