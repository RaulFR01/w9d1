<template>
  <NavBar />
  <p class="iteration2">The result of the operation is {{ result }}</p>
  <FormBonus />
  <hr />
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

<style>
.iteration1 {
  border: solid 1px green;
}
.iteration2 {
  border: solid 1px red;
}
.bonus {
  border: solid 1px blue;
}
</style>
