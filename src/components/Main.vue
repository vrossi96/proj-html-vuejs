<template>
   <div class="container-fluid">
      <Slider />
      <Jumbotron />
      <FirstSection />
      <SecondSection />
      <RightCartButtons />
      <GoTopBtn />
      <CardsSection />
   </div>
</template>

<script>
import Slider from "./Slider.vue";
import Jumbotron from "./Jumbotron.vue";
import FirstSection from "./FirstSection.vue";
import SecondSection from "./SecondSection.vue";
import RightCartButtons from "./btn-fixed/RightCartButtons.vue";
import GoTopBtn from "./btn-fixed/GoTopBtn.vue";
import CardsSection from "./CardsSection.vue";

export default {
   name: "Main",
   components: {
      Slider,
      Jumbotron,
      FirstSection,
      SecondSection,
      RightCartButtons,
      GoTopBtn,
      CardsSection,
   },
};
</script>

<style scoped lang="scss"></style>
