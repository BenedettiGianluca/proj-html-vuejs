<template>
  <section class="recentCauses">
    <div class="recentProjects">
      <div class="projects">
        <h2>RECENT CAUSES</h2>
        <hr>
        <h4>We run projects in over 30 countries in 5 contintents</h4>
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
    align-items: center;

    .recentProjects {
      display: flex;
      flex-direction: column;
      align-items: center;
      height: 75vh;
      padding: 75px 120px;

      .projects {
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
          margin: 15px 0 30px 0;
        }
    
        h4 {
          color: $RegentGray;
        }
      }

      .images {
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 60px;

        img {
          width: 280px;
          height: 210px;
          margin: 0 15px;
        }
      }
    }

    .allCauses {
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: $BurntSienna2;
      width: 100%;
      height: 15vh;

      a {
        color: white;
        font-size: 13px;
        text-decoration: none;
      }
    }
  }
</style>