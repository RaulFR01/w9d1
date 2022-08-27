<template>
  <NavBar />
  <FooterSection />
</template>

<script>
import FooterSection from "./components/footerSection.vue";
import NavBar from "./components/navBar.vue";
export default {
  name: "App",
  components: {
    FooterSection,
    NavBar,
  },
};
</script>

<style></style>
