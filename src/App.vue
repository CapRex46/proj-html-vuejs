<template>
  <div id="app">
    <header-box :navList="this.navbarList"/>
    <first-jumbo/>
    <second-jumbo/>
    <third-jumbo/>
    <fourth-jumbo/>
    <footer-box/>
    <footer-final/>
  </div>
</template>

<script>

import HeaderBox from './components/HeaderBox.vue'
import FirstJumbo from './components/FirstJumbo.vue'
import SecondJumbo from './components/SecondJumbo.vue'
import ThirdJumbo from './components/ThirdJumbo.vue'
import FourthJumbo from './components/FourthJumbo.vue'
import FooterBox from './components/FooterBox.vue'
import FooterFinal from './components/FooterFinal.vue'


export default {
  name: 'App',
  components: {
    HeaderBox,
    FirstJumbo,
    SecondJumbo,
    ThirdJumbo,
    FourthJumbo,
    FooterBox,
    FooterFinal,
  },
  data () {
    return {
      navbarList: [
        'Home',
        'About',
        'Academics',
        'Courses',
        'News',
      ],
      footinfo:[
        {
          title: 'Contact Us',
          messages: [
            '900 Wood Street, MI New York',
            '+58 325 625 000-09',
            'info@mail.com'
          ]
        },
        {
          title: 'Support Us',
          messages: [
            '> Privacy',
            '> Terms',
            '> Cookie Policy',
            '> Sitemap',
          ]
        },
        {
          title: 'Explore',
          messages: [
            '> Accomodation',
            '> Arts Academics',
            '> Central Services',
            '> Conferences and Events',
            '> Food and Drink'
          ]
        },
        {
          title: 'Visit',
          messages: [
            '> Admission',
            '> Contact Us',
            '> FAQs',
            '> Request Information',
            '> Privacy Notice',
          ]
        }
      ],
    }
  }
}
</script>

<style lang="scss">
  @import './style/main.scss';
  @import url('https://use.fontawesome.com/releases/v5.7.1/css/all.css');
</style>
