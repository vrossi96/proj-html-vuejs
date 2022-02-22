<template>
   <div class="d-flex align-items-center position-relative">
      <div role="button" class="left-arrow"><i class="fas fa-angle-left"></i></div>
      <div class="slider container">
         <div class="row">
            <!-- Left side TEXT AREA -->
            <div class="col-5 offset-1 d-flex flex-column justify-content-center">
               <h1>Devotion that never <i>ends</i></h1>
               <p class="text-secondary py-4">
                  Aperiam, similique earum. Illo alias accusamus corrupti magni quibusdam autem odio nihil. Odio eius pariatur consectetur voluptas
                  voluptates placeat reprehenderit laudantium repellat!
               </p>
               <div>
                  <a class="p-btn text-uppercase" href="#">Read more</a>
               </div>
            </div>
            <!-- RIGHT side IMG AREA -->
            <div class="img-slider col-5 offset-1 d-flex align-items-center justify-content-center">
               <img src="../assets/images/img/h-2-slider-img-15.png" alt="" />
               <img src="../assets/images/img/h-2-slider-img-16.png" alt="" />
               <!-- decorations -->
               <img class="decorations-1" src="../assets/images/img/short-slider-rev-1-img-2.png" alt="Flower" />
               <img class="decorations-2" src="../assets/images/img/h-2-slider-img-14.png" alt="Flower" />
               <img class="decorations-3" src="../assets/images/img/short-slider-rev-1-img-6.png" alt="Flower" />
               <img class="decorations-4" src="../assets/images/img/h-2-slider-img-17.png" alt="Flower" />
               <img class="decorations-5" src="../assets/images/img/h-2-slider-img-13.png" alt="Flower" />
               <img class="decorations-6" src="../assets/images/img/h-2-slider-img-12.png" alt="Flower" />
            </div>
         </div>
      </div>
      <div role="button" class="right-arrow"><i class="fas fa-angle-right"></i></div>
      <div class="dots-container d-flex align-items-center">
         <div role="button" class="dot"></div>
         <div role="button" class="dot"></div>
         <div role="button" class="dot"></div>
      </div>
   </div>
</template>

<script>
export default {
   name: "Slider",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_var.scss";
@import "../assets/scss/_mixins.scss";

[class*="fa-angle-"] {
   color: white;
   @include flex-center;
   @include eq-size(30px);
   font-size: 20px;
   border-radius: 50%;
   background-color: $bg-brown;
}

.dots-container {
   position: absolute;
   bottom: 20px;
   left: 50%;
   transform: translateX(-50%);

   .dot {
      @include eq-size(10px);
      border-radius: 50%;
      background-color: $bg-brown;
      margin: 0 5px;
      &:hover {
         transform: scale(1.5);
      }
   }
}

.slider {
   margin-top: 50px;
   margin-bottom: 40px;

   .col-5 {
      // LEFT SIDE-TEXT SECTION
      h1 {
         font-size: 75px;
         i {
            font-family: "American Typewriter", serif;
            font-weight: 600;
         }
      }

      // TODO mettere in utils per riutilizzo anche per header
      a {
         @include strong-small-txt;
      }
      .p-btn {
         padding: 15px 45px;
         border: 2px solid $b-brown;
         transition: 0.2s linear;

         &:hover {
            background-color: $bg-brown;
            color: #fff;
         }
      }
   }

   // RIGHT SIDE-IMG SECTION
   .img-slider {
      position: relative;
      img {
         height: 80%;
      }

      // DECORATIONS
      [class*="decorations"] {
         position: absolute;
         z-index: -1;
      }
      .decorations-1,
      .decorations-2,
      .decorations-3 {
         height: 60px;
      }
      .decorations-1 {
         top: 25px;
         left: -40px;
      }
      .decorations-2 {
         top: 0;
         right: 0;
      }
      .decorations-3 {
         top: 100px;
         right: -55px;
      }
      .decorations-4 {
         height: 120px;
         bottom: 45px;
         right: -100px;
      }
      .decorations-5 {
         height: 75px;
         bottom: 45px;
         left: -50px;
      }
      .decorations-6 {
         height: 40px;
         bottom: 230px;
         left: -75px;
      }
   }
}
</style>
