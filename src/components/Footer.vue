<template>
   <div class="footer">
      <div class="container">
         <div class="row">
            <div class="col-12 d-flex justify-content-between align-items-center">
               <div v-for="(comp, i) in footerMenu" :key="i" class="footer-section">
                  <img v-if="comp.img" :src="require('../assets/images/img/' + comp.img)" />
                  <p v-for="tex in comp.text" :key="tex">{{ tex }}</p>
                  <div v-if="comp.icons" class="d-flex justify-content-between">
                     <i v-for="icon in comp.icons" :key="icon" role="button" class="fab" :class="icon"></i>
                  </div>
               </div>
            </div>
         </div>
      </div>
   </div>
</template>

<script>
export default {
   name: "Footer",
   data() {
      return {
         footerMenu: [
            { img: "logo-sidearea-1.png", text: ["Let's get creative"], icons: [] },
            { img: "", text: ["maree.qode@gmail.com", "+44645 321 789"], icons: [] },
            { img: "", text: ["Avenue d'Auderghem 10", "1040 Brussels, Belgium"], icons: [] },
            { img: "", text: ["Stay in touch with us"], icons: ["fa-twitter", "fa-pinterest-p", "fa-facebook-f", "fa-linkedin-in"] },
         ],
      };
   },
};
</script>

<style scoped lang="scss">
.footer {
   background-color: #c0e1cf;
   .col-12 {
      height: 120px;
      .footer-section {
         :first-child {
            margin-bottom: 10px;
         }
      }
   }
   p {
      font-size: 14px;
      font-weight: 600;
      margin-bottom: 0;
   }
}
</style>
