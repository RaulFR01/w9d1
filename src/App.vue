<template>
  <NavBar />
  <p>The result of the operation is {{ result }}</p>
  <FormBonus />
  <FooterSection />
</template>

<script>
import FooterSection from "./components/footerSection.vue";
import NavBar from "./components/navBar.vue";
import FormBonus from "./components/formBonus.vue";
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
    FormBonus,
  },

  created() {
    this.result = 2 + 2;
  },
};
</script>

<style></style>
