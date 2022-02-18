<template>
   <div id="app">
      <Header />
   </div>
</template>

<script>
import Header from "./components/Header.vue";

export default {
   name: "App",
   components: {
      Header,
   },
};
</script>

<style lang="scss">
@import "../src/assets/scss/style.scss";
#app {
   font-family: Avenir, Helvetica, Arial, sans-serif;
   -webkit-font-smoothing: antialiased;
}
</style>
