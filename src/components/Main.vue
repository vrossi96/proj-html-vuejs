<template>
   <div class="container-fluid">
      <Slider />
      <Jumbotron />
      <FirstSection />
      <SecondSection />
      <RightCartButtons />
      <CardsSection />
   </div>
</template>

<script>
import Slider from "./Slider.vue";
import Jumbotron from "./Jumbotron.vue";
import FirstSection from "./FirstSection.vue";
import SecondSection from "./SecondSection.vue";
import RightCartButtons from "./RightCartButtons.vue";
import CardsSection from "./CardsSection.vue";

export default {
   name: "Main",
   components: {
      Slider,
      Jumbotron,
      FirstSection,
      SecondSection,
      RightCartButtons,
      CardsSection,
   },
};
</script>

<style scoped lang="scss"></style>
