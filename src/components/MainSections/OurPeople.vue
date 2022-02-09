<template>
  <section class="ourPeople">
    <div class="ourMission">
      <h2>EVERY MOMENT COUNTS</h2>
      <hr>
      <p>lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum 
         lorem ipsum lorem ipsum lorem ipsum ipsum</p>
      <p>lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum 
         lorem ipsum lorem</p>
      <p>lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum</p>
      <button type="button">OUR MISSION</button>
    </div>
    <div class="ourNumbers">
      <div>
        <i class="fa-regular fa-heart"></i>
        <span> 2032</span>
        <p>Volunteers worldwide</p>
      </div>
      <div>
        <i class="fa-solid fa-globe"></i>
        <span> 132</span>
        <p>Active projects</p>
      </div>
      <div>
        <i class="fa-solid fa-dollar-sign"></i>
        <span> 3,8M</span>
        <p>Donated</p>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'OurPeople'
  }
</script>

<style lang="scss">
  @import "../../assets/scssVariables.scss";

  .ourPeople {
    display: flex;
    height: 75vh;

    .ourMission {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: flex-start;
      width: 65vw;
      padding: 80px;

      h2, hr, p {
        margin-bottom: 26px;
      }

      h2 {
        color: $Thunder;
      }

      hr {
        color: $Goldenrod;
        width: 175px;
        border-top: 3px solid $Goldenrod;
      }

      p {
        color: $Tuna2;
        font-size: 13px;
        line-height: 28px;
      }

      button {
        background-color: $Goldenrod;
        color: white;
        border: 1px solid $Goldenrod;
      }
    }

    .ourNumbers {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background-image: url(../../assets/project_images/home-content-bg-1.jpg);
      background-size: cover;
      background-position: center;
      color: white;
      width: 35vw;
      
      div {
        padding: 33px 0;

        span, .fa-heart, .fa-globe, .fa-dollar-sign {
          font-size: 40px;
        }

        .fa-heart {
          padding-left: 18px;
        }
  
        p {
          font-size: 20px;
          text-align: center;
          margin-top: 5px;
        }
      }
    }
  }
</style>