<template>
  <NavBar />
  <p class="iteration2">The result of the operation is {{ result }}</p>
  <FormBonus />
  <hr />
  <ConditionTest />
  <hr />
  <ListData />
  <hr />
  <ChangeElementColor />
  <hr />
  <FooterSection />
</template>

<script>
import FooterSection from "./components/footerSection.vue";
import NavBar from "./components/navBar.vue";
import FormBonus from "./components/formBonus.vue";
import ConditionTest from "./components/ConditionTest.vue";
import ListData from "./components/listData.vue";
import ChangeElementColor from "./components/changeElementColor.vue";
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
    ConditionTest,
    ListData,
    ChangeElementColor,
  },

  created() {
    this.result = 2 + 2;
  },
};
</script>

<style>
.iteration1 {
  border: solid 2px green;
}
.iteration2 {
  border: solid 2px red;
}
.iteration3 {
  border: solid 2px orange;
}
.iteration4 {
  border: solid 2px pink;
}
.iteration5 {
  border: solid 2px black;
}
.bonus {
  border: solid 2px blue;
}
</style>
