<template>
   <div class="row">
      <div class="col-10 offset-1 d-flex flex-column justify-content-center">
         <h2 class="text-center">Want to work with us? Send us <i>a message</i></h2>
         <p class="text-center text-secondary py-3">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora ut sed numquam iste cupiditate odit exercitationem deleniti quo
            corporis. Natus repellendus accusantium eveniet quaerat amet nesciunt suscipit officia repudiandae quas.
         </p>
         <div class="text-center">
            <a class="p-btn text-uppercase" href="#">contact</a>
         </div>
      </div>
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
   background-color: $bg-ylight;
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
