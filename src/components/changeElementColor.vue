<template>
  <div class="iteration5">
    <p class="text" v-bind:style="{ color: activeColor }">
      This text is going to change the color randomly
    </p>
    <button @click="changeColor">Change color</button>
  </div>
</template>

<script>
export default {
  name: "changeElementColor",
  data() {
    return {
      activeColor: "blue",
    };
  },
  methods: {
    changeColor() {
      this.activeColor =
        "#" + Math.floor(Math.random() * 16777215).toString(16);
      return this.activeColor;
    },
  },
};
</script>

<style scoped></style>
