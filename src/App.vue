<template>
  <div id="app">
    
    <a name="home"></a>
    <NavMobile v-bind:class="{ open: showNav }"/>
    <Burger 
    @click.native="showNav = !showNav"
    v-if="mobileView"/>
    <div class="content" v-bind:class="{ opened: showNav }">
      <Preloader />
      <Header v-if="!mobileView"/>
      <Main />
      <Skills />
      <About />
      <Portfolio />
      <Footer />
    </div>
  </div>
</template>

<script>
import Header from './components/Header';
import Main from './components/Main';
import About from './components/About';
import Skills from './components/Skills';
import Portfolio from './components/Portfolio';
import Footer from './components/Footer';
import Burger from './components/Burger';
import NavMobile from './components/NavMobile';
import Preloader from './components/Preloader';
export default {
  name: 'App',
  components: {
    Header,
    Main,
    About,
    Skills,
    Portfolio,
    Footer,
    Burger,
    NavMobile,
    Preloader
  },
  data() {
      return {
          mobileView: true,
          showNav: false,
      }
  },
  methods: {
    handleView() {
      this.mobileView = window.innerWidth <= 768;
    }
  },
  created() {
    this.handleView();
    window.addEventListener('resize', this.handleView);
    console.log("for more info: https://www.youtube.com/watch?v=dQw4w9WgXcQ");
  }
}

</script>

<style lang="scss">
  body {
    font-family: Arial, sans-serif;
    font-size: 18px;
    background: #FFFFFF;
  }
  * {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  .content {
    position: absolute;
    top: 0;
    transition: 1s cubic-bezier(0,.12,.14,1);
  }
  .open {
    z-index: 2;
  }
  .opened {
    transform: translateX(50vw);
  }
  @media(max-width: 576px) {
    body {
      font-size: 9px;
      $main-container: 80%;
    }
  }
  @media(min-width: 576px) {
    body {
      font-size: 10px;
    }
  }
  @media(min-width: 768px) {
    body {
      font-size: 12px;
    }
  }
  @media(min-width: 992px) {
    body {
      font-size: 14px;
    }
  }
  @media(min-width: 1200x) {
    body {
      font-size: 16px;
    }
  }
</style>
