<template>
   <div>
      <div class="row">
         <!-- <div class="col-4 jum-block" :style="{ backgroundImage: `url(${require(test)})` }"></div> non va-->
         <!-- <div
            v-for="(image, index) in jumboCards"
            :key="index"
            :style="{ backgroundImage: `url(${require('../assets/images/img/' + image.img)})` }"
         ></div> -->
         <div class="col-4 jum-block" :style="{ backgroundImage: `url(${require('../assets/images/img/h-2-port-img-1.jpg')})` }"></div>
         <div class="col-4 jum-block" :style="{ backgroundImage: `url(${require('../assets/images/img/h-2-port-img-2.jpg')})` }"></div>
         <div class="col-4 jum-block" :style="{ backgroundImage: `url(${require('../assets/images/img/h-2-port-img-3.jpg')})` }"></div>
         <div class="col-4 jum-block" :style="{ backgroundImage: `url(${require('../assets/images/img/h-2-port-img-4.jpg')})` }"></div>
         <div class="col-4 jum-block" :style="{ backgroundImage: `url(${require('../assets/images/img/h-2-port-img-5.jpg')})` }"></div>
         <div class="col-4 jum-block" :style="{ backgroundImage: `url(${require('../assets/images/img/h-2-port-img-6.jpg')})` }"></div>
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
            { img: "h-2-port-img-1.jpg" },
            { img: "h-2-port-img-2.jpg" },
            { img: "h-2-port-img-3.jpg" },
            { img: "h-2-port-img-4.jpg" },
            { img: "h-2-port-img-5.jpg" },
            { img: "h-2-port-img-6.jpg" },
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
.col-4 {
   height: calc(100vw / 3);
   border: 1px solid black;
}
.jum-block {
   background-size: cover;
   background-position: center;
   background-repeat: no-repeat;
}
</style>
