<template>
  <header>
    <nav>
      <div>
        <img :src="require(`@/assets/project_images/${img}`)">
      </div>
      <div>
        <li>{{li1}}</li>
        <li>{{li2}}</li>
        <li>{{li3}}</li>
        <li>{{li4}}</li>
        <button type="button">{{button}}</button>
      </div>
    </nav>
    <section>
      <h1>MAKE A DIFFERENCE</h1>
      <p>As long as poverty, injustice & inequality persist, none of us can truly rest</p>
      <div>
        <button type="button">OUR MISSION</button>
        <button type="button">DONATE NOW</button>
      </div>
    </section>
  </header>
</template>

<script>
  export default {
    name: 'Header',
    props: {
      img: String,
      li1: String,
      li2: String,
      li3: String,
      li4: String,
      button: String
    }
  }
</script>

<style lang="scss">
  @import "../assets/scssVariables.scss";

  header {
    background-image: url('../assets/project_images/home-page-slider.jpg');
    background-size: cover;
    background-position: center;
    height: 105vh;
  
    nav {
      position: absolute;
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
        border: 1px solid $Goldenrod;
        margin-left: 30px;
      }
    }

    section {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      color: white;
      padding-top: 40vh;

      p {
        color: $FrenchGray;
        margin: 15px 0 30px 0;
      }

      button {
        background-color: rgba(0,0,0,0.0);
        color: white;
        border: 2px solid white;
        margin: 0 5px;

        &:hover {
          color: $Goldenrod;
          border-color: $Goldenrod;
        }
      }
    }
  }
</style>