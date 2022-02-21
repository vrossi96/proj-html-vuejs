<template>
   <div class="container-fluid" id="header">
      <div class="nav row h-100 align-items-center justify-content-between">
         <!-- Left header with logo -->
         <div class="col flex-grow-0">
            <img role="button" src="../assets/images/img/logo-sidearea-1.png" alt="Logo" />
         </div>
         <!-- RIGHT header with nav -->
         <ul class="col flex-grow-0">
            <li role="button" v-for="item in links" :key="item.name" class="text-uppercase mx-3 d-flex align-items-center">
               <span v-if="!item.img">{{ item.name }}</span>
               <img v-else :src="require(`../assets/images/svg/${item.img}`)" :alt="item.name" />
            </li>
         </ul>
      </div>
   </div>
</template>

<script>
export default {
   name: "Header",
   props: {},
   data() {
      return {
         links: [
            { name: "home", url: "#", img: "" },
            { name: "pages", url: "#", img: "" },
            { name: "portfolio", url: "#", img: "" },
            { name: "blog", url: "#", img: "" },
            { name: "shop", url: "#", img: "" },
            { name: "elements", url: "#", img: "" },
            { name: "more", url: "#", img: "svg-1.svg" },
         ],
      };
   },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_mixins.scss";
#header {
   height: 96px;

   span {
      @include strong-normal-txt;
   }

   ul {
      list-style: none;
      display: flex;
      margin-bottom: 0;
   }
}
</style>
