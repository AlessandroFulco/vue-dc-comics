<template>
    <div id="app">
      <HeaderNavbar/>
      <MainContent/>
      <FooterPage/>
    </div>
</template>

<script>
import HeaderNavbar from './components/HeaderNavbar.vue'
import MainContent from './components/MainContent.vue'
import FooterPage from './components/FooterPage.vue'

export default {
  name: 'App',
  components: {
    HeaderNavbar,
    MainContent,
    FooterPage
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
