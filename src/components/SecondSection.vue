<template>
   <div class="row">
      <div class="second-section col-10 offset-1 d-flex flex-column justify-content-center">
         <h2 class="text-center">Want to work with us? Send us <i>a message</i></h2>
         <p class="text-center text-secondary py-3">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora ut sed numquam iste cupiditate odit exercitationem deleniti quo
            corporis. Natus repellendus accusantium eveniet quaerat amet nesciunt suscipit officia repudiandae quas.
         </p>
         <div class="text-center">
            <a class="p-btn text-uppercase" href="#">contact</a>
         </div>
      </div>
      <img class="decoration-1" src="../assets/images/img/short-slider-rev-1-img-5.png" alt="Nature" />
      <img class="decoration-2" src="../assets/images/img/short-slider-rev-1-img-5.png" alt="Nature" />
      <img class="decoration-3" src="../assets/images/img/short-slider-rev-1-img-5.png" alt="Nature" />
      <img class="decoration-4" src="../assets/images/img/short-slider-rev-1-img-5.png" alt="Nature" />
      <img class="decoration-5" src="../assets/images/img/short-slider-rev-1-img-5.png" alt="Nature" />
      <img class="decoration-6" src="../assets/images/img/short-slider-rev-1-img-5.png" alt="Nature" />
      <img class="decoration-7" src="../assets/images/img/short-slider-rev-1-img-2.png" alt="Nature" />
      <img class="decoration-8" src="../assets/images/img/short-slider-rev-1-img-6.png" alt="Nature" />
   </div>
</template>

<script>
export default {
   name: "SecondSection",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_var.scss";
@import "../assets/scss/_mixins.scss";

.row {
   position: relative;
   overflow: hidden;
   background-color: $bg-ylight;
   // decorations
   > img {
      position: absolute;
      padding: 0;
      margin: 0;
      &.decoration-1,
      &.decoration-2,
      &.decoration-3,
      &.decoration-4 {
         transform: rotate(180deg);
      }
      &.decoration-2,
      &.decoration-5,
      &.decoration-6 {
         filter: brightness(0) saturate(100%) invert(98%) sepia(2%) saturate(7500%) hue-rotate(324deg) brightness(118%) contrast(77%);
      }
      &.decoration-3,
      &.decoration-4,
      &.decoration-5,
      &.decoration-6 {
         width: 500px;
         height: 200px;
      }
      &.decoration-1 {
         width: 540px;
         height: 150px;
         top: -75px;
         left: -130px;
      }
      &.decoration-2 {
         width: 340px;
         height: 124px;
         top: -80px;
         left: 165px;
      }
      &.decoration-3 {
         top: -105px;
         right: -225px;
      }
      &.decoration-4 {
         filter: brightness(0) saturate(100%) invert(93%) sepia(14%) saturate(193%) hue-rotate(95deg) brightness(99%) contrast(91%);
         top: -154px;
         right: -24px;
      }
      &.decoration-5 {
         bottom: -133px;
         right: -100px;
      }
      &.decoration-6 {
         bottom: -168px;
         left: 100px;
      }
      &.decoration-7,
      &.decoration-8 {
         filter: brightness(0) saturate(100%) invert(92%) sepia(40%) saturate(525%) hue-rotate(295deg) brightness(100%) contrast(91%);
         @include eq-size(50px);
      }
      &.decoration-7 {
         right: 180px;
         top: 70px;
      }
      &.decoration-8 {
         bottom: 20px;
         left: 100px;
      }
   }

   .col-10 {
      height: 400px;
   }

   h2 {
      font-size: 60px;
      i {
         font-family: "American Typewriter", serif;
         font-weight: 600;
      }
   }

   // BTN
   a {
      @include strong-small-txt;
      background-color: $bg-aqualight;
   }
   .p-btn {
      padding: 15px 45px;
      border: 2px solid $b-aqualight;
      transition: 0.2s linear;
      &:hover {
         color: #fff;
         background-color: $bg-brown;
         border-color: $b-brown;
      }
   }
}
</style>
