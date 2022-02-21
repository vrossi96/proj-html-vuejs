<template>
   <div class="footer">
      <div class="container">
         <div class="row">
            <div class="col-12 d-flex justify-content-between align-items-center">
               <div class="footer-section">
                  <img src="../assets/images/img/logo-sidearea-1.png" alt="" />
                  <p>Let's get creative</p>
               </div>
               <div class="footer-section">
                  <p>maree.qode@gmail.com</p>
                  <p>+44645 321 789</p>
               </div>
               <div class="footer-section">
                  <p>Avenue d'Auderghem 10</p>
                  <p>1040 Brussels, Belgium</p>
               </div>
               <div class="footer-section">
                  <p>Stay in touch with us</p>
                  <div class="d-flex justify-content-between">
                     <i role="button" class="fab fa-twitter"></i>
                     <i role="button" class="fab fa-pinterest-p"></i>
                     <i role="button" class="fab fa-facebook-f"></i>
                     <i role="button" class="fab fa-linkedin-in"></i>
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
