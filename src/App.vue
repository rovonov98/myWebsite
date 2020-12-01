<template>
  <div id="app">
    <Header />
    <Main />
    <Skills />
    <About />
    <Portfolio />
    <Contacts />
  </div>
</template>

<script>
import Header from './components/Header';
import Main from './components/Main';
import About from './components/About';
import Skills from './components/Skills';
import Portfolio from './components/Portfolio';
import Contacts from './components/Contacts';
export default {
  name: 'App',
  components: {
    Header,
    Main,
    About,
    Skills,
    Portfolio,
    Contacts
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
  @media(max-width: 576px) {
    body {
      font-size: 7px;
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
