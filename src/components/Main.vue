<template>
   <div class="container-fluid">
      <Slider />
      <Jumbotron />
      <FirstSection />
      <RightCartButtons />
   </div>
</template>

<script>
import Slider from "./Slider.vue";
import Jumbotron from "./Jumbotron.vue";
import FirstSection from "./FirstSection.vue";
import RightCartButtons from "./RightCartButtons.vue";

export default {
   name: "Main",
   components: {
      Slider,
      Jumbotron,
      FirstSection,
      RightCartButtons,
   },
};
</script>

<style scoped lang="scss"></style>
