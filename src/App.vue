<template>
    <div id="app">
      <HeaderNavbar/>
      <div class="bg-main-content">
        <MainContent/>
      </div>
      <OtherContent/>
      <FooterPage/>
    </div>
</template>

<script>
import HeaderNavbar from './components/HeaderNavbar.vue'
import MainContent from './components/MainContent.vue'
import OtherContent from './components/OtherContent.vue'
import FooterPage from './components/FooterPage.vue'

export default {
  name: 'App',
  components: {
    HeaderNavbar,
    MainContent,
    OtherContent,
    FooterPage
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing:border-box
}
#app {
  font-family: arial, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  .bg-main-content {
    background-color: #000;
  }
}
</style>
