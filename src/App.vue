<template>
  <div id="app">
    <header-box :navList="navbarList" />
    <first-jumbo/>
    <second-jumbo/>
    <third-jumbo/>
    <fourth-jumbo/>
    <footer-box/>
    <footer-final/>
    <footer-array :footlink="footinfo"/>
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
import FooterArray from './components/FooterArray.vue'



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
    FooterArray,
  },
  data () {
    return {
      navbarList: [
        {
          navtxt:'Home',
        },
        {
          navtxt: 'About',
        },
        {
          navtxt: 'Academics',
        },
        {
          navtxt: 'Courses',
        },
        {
          navtxt: 'News',
        }
      ],
      footinfo:[
        {
          title: 'Contact Us',
          msg1: "900 Wood Street, MI New York",
          msg2:'+58 325 625 000-09',
          msg3:'info@mail.com',
          msg4: '',
          msg5: '',
          msg6: '',
        },
        {
          title: 'Support Us',
          msg1:'> Privacy',
          msg2:'> Terms',
          msg3:'> Cookie Policy',
          msg4: '> Sitemap',
          msg5: '',
          msg6: '',                    
        },
        {
          title: 'Explore',
          msg1:  '> Accomodation',
          msg2:  '> Arts Academics',
          msg3:  '> Central Services',
          msg5:  '> Conferences and Events',
          msg6:  '> Food and Drink',
        },
        {
          title: 'Visit',
          msg1:  '> Admission',
          msg2:  '> Contact Us',
          msg3:  '> FAQs',
          msg4:  '> Request Information',
          msg5:  '> Privacy Notice',
          msg6: '',
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
