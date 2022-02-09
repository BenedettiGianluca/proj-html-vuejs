<template>
  <section class="ourValues">
    <div class="unattainableSky">
    </div>
    <div class="bigValues">
      <div class="values">
        <h2>OUR VALUES</h2>
        <hr>
        <h4>Think Big. Act Bigger.</h4>
      </div>
      <div class="civilization">
        <div>
          <i class="fa-solid fa-droplet"></i>
          <h4>Clean Water</h4>
          <p>lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum</p>
          <button type="button">LEARN MORE</button>
        </div>
        <div>
          <i class="fa-solid fa-stethoscope"></i>
          <h4>Vaccinations</h4>
          <p>lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum</p>
          <button type="button">LEARN MORE</button>
        </div>
        <div>
          <i class="fa-solid fa-graduation-cap"></i>
          <h4>Education</h4>
          <p>lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum</p>
          <button type="button">LEARN MORE</button>
        </div>
        <div>
          <i class="fa-brands fa-pagelines"></i>
          <h4>Farming</h4>
          <p>lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum</p>
          <button type="button">LEARN MORE</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'OurValues'
  }
</script>

<style lang="scss">
  @import "../../assets/scssVariables.scss";

  .ourValues {

    .unattainableSky {
      background-image: url(../../assets/project_images/home-content-bg-2.jpg);
      background-size: cover;
      background-position: top;
      height: 17vh;
    }

    .bigValues {
      display: flex;
      flex-direction: column;
      align-items: center;
      background-image: url(../../assets/project_images/home-content-bg-2.jpg);
      background-position: center;
      height: 73vh;
      padding: 0 170px 150px 170px;
  
      h4 {
        color: white;
        font-size: 21px;
      }
  
      .values {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        color: white;
        margin-bottom: 105px;
  
        hr {
          color: $Goldenrod;
          width: 125px;
          border-top: 3px solid $Goldenrod;
          margin: 18px 0 30px 0;
        }
      }
  
      .civilization {
        display: flex;
        justify-content: space-around;
        align-items: center;
  
        div {
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: center;
          margin: 0 7px;
  
          .fa-droplet, .fa-stethoscope, .fa-graduation-cap, .fa-pagelines {
            color: $Goldenrod;
            font-size: 55px;
            margin-bottom: 10px;
          }

          h4 {
            margin-bottom: 17px;
          }

          p {
            color: $FrenchGray;
            font-size: 13px;
            line-height: 28px;
            margin-bottom: 25px;
          }
  
          button {
            background-color: $Goldenrod;
            color: white;
            border: 1px solid $Goldenrod;
          }
        }
      }
    }
  }
</style>