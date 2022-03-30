<template>
  <div id="app">
    <Header />
    <CoverList />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import CoverList from './components/CoverList.vue'



export default {
  name: 'App',
  components: {
    Header,
    CoverList
  }
}
</script>

<style lang="scss">

*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;

}
</style>
