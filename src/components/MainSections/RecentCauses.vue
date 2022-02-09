<template>
  <section class="recentCauses">
    <div class="recentProjects">
      <div class="projects">
        <h2>RECENT CAUSES</h2>
        <hr>
        <p>We run projects in over 30 countries in 5 contintents</p>
      </div>
      <div class="images">
        <img src="../../assets/project_images/avada-charity-fair-trade-featured.jpg">
        <img src="../../assets/project_images/avada-charity-shelter-featured.jpg">
        <img src="../../assets/project_images/avada-charity-farming-featured.jpg">
        <img src="../../assets/project_images/avada-charity-vaccines-featured.jpg">
      </div>
    </div>
    <div class="allCauses">
      <a href="#">VIEW ALL OUR CAUSES</a>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'RecentCauses'
  }
</script>

<style lang="scss">
   @import "../../assets/scssVariables.scss";

  .recentCauses {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .recentProjects {
      display: flex;
      flex-direction: column;
      align-items: center;
      height: 70vh;
      padding: 100px 120px;

      .project {
        display: flex;
        flex-direction: column;
        align-items: center;

        h2 {
          color: $Thunder;
        }
        
        hr {
          color: $Goldenrod;
          width: 125px;
          border-top: 3px solid $Goldenrod;
          margin: 18px 0 30px 0;
        }
    
        p {
          color: $Tuna2;
        }
      }

      .images {
        display: flex;
        justify-content: center;
        align-items: center;

        img {
          width: 200px;
          height: 150px;
          margin: 0 25px;
        }
      }
    }

    .allCauses {
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: $BurntSienna2;
      width: 100vw;
      height: 15vh;

      a {
        color: white;
        font-size: 15px;
        text-decoration: none;
      }
    }
  }
</style>