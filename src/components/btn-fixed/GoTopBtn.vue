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

.go-on-top {
   position: fixed;
   right: 20px;
   bottom: 20px;
   a {
      display: flex;
      justify-content: center;
      padding: 10px;
      height: 40px;
      width: 40px;
      background-color: $bg-aqua;
   }
}
</style>
