<template>
   <div class="cart-buttons">
      <div><img src="../assets/images/svg/svg-4.svg" alt="Wheel" /></div>
      <div><img src="../assets/images/svg/svg-6.svg" alt="Cart" /></div>
   </div>
</template>

<script>
export default {
   name: "RightCartButtons",
};
</script>

<style scoped lang="scss">
.cart-buttons {
   position: fixed;
   right: 0;
   top: 50%;

   & > * {
      height: 40px;
      width: 40px;
      padding: 10px;
      cursor: pointer;
   }

   div:first-child {
      background-color: #ef2853;
      margin-bottom: 10px;
   }
   div:last-child {
      background-color: #fff;
   }
}
</style>
