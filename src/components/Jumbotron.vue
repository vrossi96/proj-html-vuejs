<template>
   <div>
      <div class="row">
         <div
            class="col-4 jum-block d-flex align-items-center"
            v-for="(image, index) in jumboCards"
            :key="index"
            :style="{ backgroundImage: `url(${require('../assets/images/img/' + image.img)})` }"
         >
            <div class="row">
               <div class="col box-label">
                  <h4>{{ image.title }}</h4>
                  <i>{{ image.type }}</i>
               </div>
            </div>
         </div>
      </div>
   </div>
</template>

<script>
export default {
   name: "Jumbotron",
   data() {
      return {
         test: "../assets/images/img/h-2-port-img-1.jpg",
         cardImgPath: "../assets/images/img/",
         jumboCards: [
            { img: "h-2-port-img-1.jpg", title: "Letters", type: "Illustration" },
            { img: "h-2-port-img-2.jpg", title: "Couple bycicle", type: "Movement" },
            { img: "h-2-port-img-3.jpg", title: "US letters Brochure Template", type: "Books" },
            { img: "h-2-port-img-4.jpg", title: "Illustration of novels", type: "Illustration" },
            { img: "h-2-port-img-5.jpg", title: "Van Gogh phone wallpaper", type: "Phone art" },
            { img: "h-2-port-img-6.jpg", title: 'Google "art" with letters', type: "Example" },
         ],
      };
   },
   computed: {
      bgImg() {
         return this.cane;
      },
   },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_mixins.scss";

.col-4 {
   height: calc(100vw / 3);
}
.jum-block {
   background-size: cover;
   background-position: center;
   background-repeat: no-repeat;
   cursor: pointer;

   .box-label {
      opacity: 0;
      background-color: #fff;
      padding: 15px 25px;
      transition: 0.2s linear;

      i {
         font-family: "American Typewriter", serif;
         font-weight: 600;
      }
   }

   &:hover {
      .box-label {
         opacity: 1;
      }
   }
}
</style>
