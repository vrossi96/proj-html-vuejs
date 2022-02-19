<template>
   <div class="container-fluid">
      <Slider />
      <Jumbotron />
      <FirstSection />
   </div>
</template>

<script>
import Slider from "./Slider.vue";
import Jumbotron from "./Jumbotron.vue";
import FirstSection from "./FirstSection.vue";

export default {
   name: "Main",
   components: {
      Slider,
      Jumbotron,
      FirstSection,
   },
};
</script>

<style scoped lang="scss"></style>
