<template>
   <div class="go-on-top">
      <a href="#header"><img src="../../assets/images/svg/svg-2.svg" alt="Arrow top" /></a>
   </div>
</template>

<script>
export default {
   name: "GoTopBtn",
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/_var.scss";
@import "../../assets/scss/_mixins.scss";

.go-on-top {
   position: fixed;
   @include equal-distance-rb(20px);
   a {
      display: flex;
      justify-content: center;
      padding: 10px;
      @include eq-size(40px);
      background-color: $bg-aqua;
   }
}
</style>
