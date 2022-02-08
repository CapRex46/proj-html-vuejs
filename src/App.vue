<template>
  <div id="app">
    <header-box/>
    <first-jumbo/>
    <second-jumbo/>
    <third-jumbo/>
    <fourth-jumbo/>
  </div>
</template>

<script>

import HeaderBox from './components/HeaderBox.vue'
import FirstJumbo from './components/FirstJumbo.vue'
import SecondJumbo from './components/SecondJumbo.vue'
import ThirdJumbo from './components/ThirdJumbo.vue'
import FourthJumbo from './components/FourthJumbo.vue'



export default {
  name: 'App',
  components: {
    HeaderBox,
    FirstJumbo,
    SecondJumbo,
    ThirdJumbo,
    FourthJumbo,
  }
}
</script>

<style lang="scss">
  @import './style/main.scss';
  @import url('https://use.fontawesome.com/releases/v5.7.1/css/all.css');
</style>
