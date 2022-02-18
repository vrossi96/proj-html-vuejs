<template>
   <div class="slider container">
      <div class="row">
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
         <div class="col-5"></div>
      </div>
   </div>
</template>

<script>
export default {
   name: "Slider",
};
</script>

<style scoped lang="scss">
.slider {
   border: 1px dashed black;

   .col-5 {
      border: 1px dotted red;
      height: 500px;

      h1 {
         font-size: 75px;
         i {
            font-family: "American Typewriter", serif;
            font-weight: 600;
         }
      }

      // TODO mettere in utils per riutilizzo anche per header
      a {
         text-decoration: none;
         font-size: 12px;
         color: #000;
      }
      .p-btn {
         padding: 15px 30px;
         border: 2px solid black;
      }
   }
}
</style>
