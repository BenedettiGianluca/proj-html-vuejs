<template>
  <footer>
    <div>
      <img src="../assets/project_images/avada-charity-sticky-header-logo.png">
    </div>
    <div class="copyrightContatti">
      <span><i class="fa-regular fa-copyright"></i> Copyright 2012 - 2020 AVADA THEME BY THEME FUSION | ALL RIGHTS RESERVED | POWERED BY WORDPRESS</span>
      <div class="contatti">
        <div><i class="fa-brands fa-facebook-f"></i></div>
        <div><i class="fa-brands fa-instagram"></i></div>
        <div><i class="fa-brands fa-twitter"></i></div>
        <div><i class="fa-brands fa-youtube"></i></div>
      </div>
    </div>
    <div class="presuntoMenuFooter"><i :class="iconaFooter"></i></div>
  </footer>
</template>

<script>
  export default {
    name: 'Footer',
    props: {
      iconaFooter: String
    }
  }
</script>

<style lang="scss">
  @import "../assets/scssVariables.scss";

  footer {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;

    img {
      transform: scale(0.66);
      margin: 20px 0;
    }

    .copyrightContatti {
      display: flex;
      flex-direction: column;
      align-items: center;
      background-color: #f5f5f5;
      width: 100vw;
      height: 15vh;

      .fa-copyright, span {
        color: $FrenchGray;
        font-size: 9px;
        padding: 20px;
      }

      .fa-copyright {
        padding: 0;
      }

      .contatti {
        display: flex;

        div {
          background-color: white;
          text-align: center;
          width: 40px;
          height: 40px;
          padding-top: 10px;
          border-radius: 50px;
          margin: 5px 3px 0 3px;

          &:hover {
            cursor: pointer;
          }
        }

        .fa-facebook-f, .fa-instagram, .fa-twitter, .fa-youtube {
          color: $Goldenrod;
          font-size: 20px;
        }
      }
    }

    .presuntoMenuFooter {
      position: absolute;
      bottom: 0;
      right: 60px;
      background-color: #464646;
      color: white;
      font-size: 15px;
      text-align: center;
      height: 30px;
      width: 35px;
      padding-top: 3.5px;
      border-radius: 5px 5px 0 0;

      &:hover {
        cursor: pointer;
      }
    }
  }
</style>