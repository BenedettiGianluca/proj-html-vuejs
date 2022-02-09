<template>
  <div id="app">
    <nav>
      <div>
        <img src="./assets/project_images/avada-charity-logo.png">
      </div>
      <div>
        <li>HOME</li>
        <li>MISSION</li>
        <li>CAUSES</li>
        <li>JOURNAL</li>
        <button type="button">DONATE</button>
      </div>
    </nav>
    <Header />
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

  p {
    font-size: 15px;
  }

  li:hover, button:hover {
    cursor: pointer;
  }

  nav {
    position: fixed;
    top: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 88vw;
    margin: 3vh 9.5vw 0 2.5vw;

    img {
      transform: scale(0.66);
    }

    li {
      display: inline;
      color: $FrenchGray;
      margin: 0 30px;

      &:hover {
        color: $Goldenrod;
      }
    }

    button {
      background-color: $Goldenrod;
      color: white;
      padding: 9px 18px;
      border: 1px solid $Goldenrod;
      margin-left: 30px;
    }
  }
</style>
