<template>
  <section class="changeToday">
    <h2>CHANGE A LIFE TODAY</h2>
    <hr>
    <p>As long as poverty, injustice & inequality persist, none of us can truly rest. It doesn't take much to change a life.
       Get in touch today and start making the difference.</p>
    <div>
      <button type="button">VOLUNTEER</button>
      <button type="button">DONATE NOW</button>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'ChangeToday'
  }
</script>

<style lang="scss">
  @import "../../assets/scssVariables.scss";

  .changeToday {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-image: url(../../assets/project_images/home-footer.jpg);
    background-size: cover;
    background-position: center;
    color: white;
    height: 60vh;
    padding: 15vh 25vw;
    
    hr {
      color: $Goldenrod;
      width: 180px;
      border-top: 3px solid $Goldenrod;
      margin: 15px 0 30px 0;
    }

    p {
      font-size: 19px;
      text-align: center;
      line-height: 28px;
    }

    div {
      display: flex;
      justify-content: center;
    
      button {
        background-color: rgba(0,0,0,0.0);
        color: white;
        border: 2px solid white;
        margin: 35px 15px;
  
        &:hover {
          color: $Goldenrod;
          border-color: $Goldenrod;
        }
      }
    }
  }
</style>