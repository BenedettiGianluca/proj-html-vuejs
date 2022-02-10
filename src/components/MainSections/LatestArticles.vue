<template>
  <section class="latestArticles">
    <div class="encouragingPhrase">
      <h2>LATEST ARTICLES</h2>
      <hr>
      <p>Together we make all the difference</p>
    </div>
    <div class="articles">
      <div class="featuredArticle">
        <div>
          <img src="../../assets/project_images/photo-1444213007800-cff19e1677ac.jpg">
        </div>
        <div>
          <a href="#">Understanding community complexities</a>
          <p>lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum</p>
        </div>
      </div>
      <SideArticles />
    </div>
    <div class="allArticles">
      <button type="button">VIEW ALL OUR ARTICLES</button>
    </div>
  </section>
</template>

<script>
  import SideArticles from './SideArticles/SideArticles.vue';

  export default {
    name: 'LatestArticles',
    components: {
      SideArticles
    }
  }
</script>

<style lang="scss">
  @import "../../assets/scssVariables.scss";

  .latestArticles {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 105vh;
    padding: 80px 0;

    .encouragingPhrase {
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
    
      p {
        color: $Tuna2;
      }
    }

    .articles {
      display: flex;
      margin: 50px 0;

      a {
        color: $Goldenrod;
        font-size: 15px;
        text-decoration: none;
      }

      p {
        color: $Tuna2;
        font-size: 13px;
        line-height: 28px;
      }
        
      .featuredArticle {
        margin-right: 30px;

        div:first-child , div:first-child >img {
          width: 360px;
          height: 270px;
        }

        div:last-child {
          width: 360px;
          padding: 15px;
          border: 1px solid $FrenchGray;
        }
      }

      .sideArticles {
        
        .sideArticle {
          display: flex;

          div:first-child , div:first-child >img {
            width: 100px;
            height: 75px;
          }
  
          div:last-child {
            width: 360px;
            padding: 2px 15px;
            margin-bottom: 22.5px;
          }
        }
      }
    }

    .allArticles {
      
      button {
        background-color: $BurntSienna2;
        color: white;
        font-size: 12px;
        padding: 9px 350px;
        border: 1px solid $BurntSienna2;
      }
    }
  }
</style>