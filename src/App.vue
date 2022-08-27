<template>
  <NavBar />
  <p>The result of the operation is {{ result }}</p>
  <FooterSection />
</template>

<script>
import FooterSection from "./components/footerSection.vue";
import NavBar from "./components/navBar.vue";
export default {
  name: "App",
  data: function () {
    return {
      result: 0,
    };
  },
  components: {
    FooterSection,
    NavBar,
  },

  created() {
    this.result = 2 + 2;
  },
};
</script>

<style></style>
