<template>
  <div id="app">
    <TheHeader />
    <MainSection />
    <BlueSection />
    <TheFooter />
    <SocialFooter />
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import BlueSection from "./components/BlueSection.vue"
import TheFooter from "./components/TheFooter.vue";
import SocialFooter from "./components/SocialFooter.vue";
import MainSection from "./components/MainSection.vue";

export default {
  name: "App",
  components: {
    TheHeader,
    BlueSection,
    TheFooter,
    SocialFooter,
    MainSection
},
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Asap+Condensed:wght@400;600;700&display=swap");
#app {
  font-family: "Asap Condensed", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
