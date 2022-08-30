<template>
  <div class="bonus">
    <p><b>This is my form</b></p>
    <form action="">
      <fieldset>
        <input type="text" v-model="name" />
      </fieldset>
      <fieldset>
        <input type="mail" v-model="email" />
      </fieldset>
    </form>

    <p><b>This is the two-way-data-binding result</b></p>

    <p>Your name is: {{ name }}</p>
    <p>Your email is: {{ email }}</p>
  </div>
</template>

<script>
export default {
  name: "formBous",
  data: function () {
    return {
      name: "",
      email: "",
    };
  },
};
</script>

<style></style>
