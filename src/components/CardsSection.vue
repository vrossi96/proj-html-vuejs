<template>
   <div class="container">
      <div class="row py-5">
         <div v-for="(card, i) in cardsDetails" :key="i" class="col-4 single-card">
            <div class="img-box">
               <img class="img-fluid" :src="require(`../assets/images/img/${card.img}`)" :alt="i" />
               <div class="label">
                  <div class="label-number text-center">
                     <i>{{ card.label.number }}</i>
                  </div>
                  <div class="label-year">
                     <p class="text-uppercase text-center m-0 pb-2">{{ card.label.year }}</p>
                  </div>
                  <div class="position-relative">
                     <div class="left-triangle"></div>
                     <div class="right-triangle"></div>
                  </div>
               </div>
            </div>
            <h4 class="py-3 m-0">{{ card.details }}</h4>
            <p>
               <i>By {{ card.author }}</i>
            </p>
         </div>
      </div>
   </div>
</template>

<script>
export default {
   name: "CardsSection",
   data() {
      return {
         cardsDetails: [
            {
               img: "h-2-blog-img-1.jpg",
               details: "This way, loves: a detailed guide through new design",
               author: "Emily Fields",
               label: {
                  number: "07",
                  year: `May'19`,
               },
            },
            {
               img: "h-2-blog-img-2.jpg",
               details: "I try to give people a different way of looking art",
               author: "Emily Fields",
               label: {
                  number: "07",
                  year: `May'19`,
               },
            },
            {
               img: "h-2-blog-img-3.jpg",
               details: "Introduce Richard Laperrière of those amazing features",
               author: "Emily Fields",
               label: {
                  number: "07",
                  year: `May'19`,
               },
            },
         ],
      };
   },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_var.scss";

.single-card {
   i {
      font-family: "American Typewriter", serif;
      font-weight: 600;
   }

   .img-box {
      position: relative;

      .label {
         position: absolute;
         left: 15px;
         top: -15px;
         box-shadow: 3px 10px 10px 0px rgba(0, 0, 0, 0.33);

         width: 50px;
         .label-number {
            background-color: $bg-aqua;
            i {
               font-size: 25px;
            }
         }
         .label-year {
            background-color: $bg-pink;
            p {
               font-size: 11px;
               font-weight: 600;
            }
         }
         [class$="t-triangle"] {
            position: absolute;
            top: 0;
            display: inline-block;
            width: 0;
            height: 0;
            border-style: solid;
         }
         .right-triangle {
            right: 0;
            border-width: 0 25px 10px 0;
            border-color: transparent $bg-pink transparent transparent;
         }
         .left-triangle {
            left: 0;
            border-width: 10px 25px 0 0;
            border-color: $bg-pink transparent transparent transparent;
         }
      }
   }
}
</style>
