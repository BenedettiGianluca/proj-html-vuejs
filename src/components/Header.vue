<template>
  <header>

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
    name: 'Header'
  }
</script>

<style lang="scss">
  @import "../assets/scssVariables.scss";

  header {
    background-image: url('../assets/project_images/home-page-slider.jpg');
    background-size: cover;
    background-position: center;
    height: 105vh;
  
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
        color: $FrenchGray;
        padding: 9px 18px;
        border: 1px solid white;
        margin: 0 5px;

        &:hover {
          color: $Goldenrod;
          border-color: $Goldenrod;
        }
      }
    }
  }
</style>