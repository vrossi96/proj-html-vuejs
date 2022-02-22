<template>
   <div class="container py-5">
      <h2 class="text-center pt-5 pb-5">Working <i>process</i></h2>
      <div class="circles-box d-flex justify-content-between pb-5">
         <div class="d-flex flex-column align-items-center">
            <div class="icon-circle">
               <i class="fas fa-lightbulb"></i>
            </div>
            <h5>First there is an idea</h5>
            <p class="text-secondary text-center">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
         </div>
         <div class="d-flex flex-column align-items-center">
            <div class="icon-circle">
               <i class="far fa-comment"></i>
            </div>
            <h5>Then we talk about</h5>
            <p class="text-secondary text-center">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
         </div>
         <div class="d-flex flex-column align-items-center">
            <div class="icon-circle">
               <i class="fas fa-cloud"></i>
            </div>
            <h5>And we think about</h5>
            <p class="text-secondary text-center">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
         </div>
         <div class="d-flex flex-column align-items-center">
            <div class="icon-circle">
               <i class="fas fa-pencil-ruler"></i>
            </div>
            <h5>So we draw along</h5>
            <p class="text-secondary text-center">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
         </div>
         <img class="bg" src="../assets/images/svg/svg-3.svg" alt="" />
      </div>
   </div>
</template>

<script>
export default {
   name: "FirstSection",
};
</script>

<style scoped lang="scss">
.container {
   h2 {
      font-size: 60px;
      i {
         font-family: "American Typewriter", serif;
         font-weight: 600;
      }
   }
   .circles-box {
      position: relative;
      p {
         padding: 0 10px;
      }

      div:nth-of-type(1) {
         i {
            color: #c0e1cf;
         }
      }
      div:nth-of-type(2) {
         i {
            color: #f8d12d;
         }
      }
      div:nth-of-type(3) {
         i {
            color: #80465f;
         }
      }
      div:nth-of-type(4) {
         i {
            color: #eb6950;
         }
      }
   }
   .icon-circle {
      i {
         font-size: 30px;
         display: block;
      }
      padding: 50px;
      border-radius: 50%;
      background-color: #faf7f1;
   }
   h5 {
      padding: 15px 0;
      font-weight: 600;
   }
   p {
      font-size: 14px;
   }
   img.bg {
      position: absolute;
      z-index: -1;
      width: 80%;
      top: 0;
      left: 0;
      transform: translateX(10%);
   }
}
</style>
