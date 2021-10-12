<template>
  <div id="app">
    <Header :navLinks="navLinks" />
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  
  components: {
    Header,
    Footer,
    Main
  },

  data() {
    return {
      
      // Nav Menu
      navLinks: [
        {
          url: '#',
          text: 'Home'
        },
        {
          url: '#',
          text: 'Apple'
        },
        {
          url: '#',
          text: 'Microsoft'
        },
        {
          url: '#',
          text: 'Android'
        },
        {
          url: '#',
          text: 'Forums'
        },
        {
          url: '#',
          text: 'Contact us'
        }
      ]
    }
  },
}
</script>

<style lang="scss">
  @import './assets/style/common.scss';
  ul {
    cursor: pointer;
  }
  li {
    list-style: none;
  }
  a {
    text-decoration: none;
  }
</style>
