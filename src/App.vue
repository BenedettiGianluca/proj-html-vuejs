<template>
  <div id="app">
    <Header :img="navElements.img" :li1="navElements.li1" :li2="navElements.li2" :li3="navElements.li3" :li4="navElements.li4" :button="navElements.button"/>
    <Main />
    <Footer />
  </div>
</template>

<script>
  import Header from './components/Header.vue';
  import Main from './components/Main.vue';
  import Footer from './components/Footer.vue';
  
  export default {
    name: 'App',
    components: {
      Header,
      Main,
      Footer
    },
    data(){
      return{
        navElements: {
          img: 'avada-charity-logo.png',
          li1: 'HOME',
          li2: 'MISSION',
          li3: 'CAUSES',
          li4: 'JOURNAL',
          button: 'DONATE'
        }
      }
    }
  }
</script>

<style lang="scss">
  @import "./assets/scssVariables.scss";

  * {
    box-sizing: border-box;
    border: 0;
    margin: 0;
    font-family: 'Roboto Condensed', sans-serif;
    font-size: 10px;
  }

  h1 {
    font-size: 38px;
  }

  h2 {
    font-size: 33px;
  }

  p {
    font-size: 14px;
  }

  button {
    padding: 9px 20px;
  }

  li:hover, button:hover {
    cursor: pointer;
  }
</style>