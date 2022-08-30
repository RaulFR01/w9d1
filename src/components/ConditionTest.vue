<template>
  <div class="iteration3">
    <div v-if="condition === true">
      <p>Estoy dentro del div porque la variables condition es true</p>
    </div>

    <div v-else>
      <p>Estoy dentro del div porque la variable condition es false</p>
    </div>

    <button v-on:click="condition = !condition">Cambiar condicion</button>
  </div>
</template>

<script>
export default {
  name: "ConditionTest",
  data() {
    return {
      condition: true,
    };
  },
};
</script>

<style></style>
