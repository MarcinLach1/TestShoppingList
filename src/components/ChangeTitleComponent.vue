<template>
  <div>
    <em>Zmiana tytułu listy: </em>
    <input v-bind:value="value" v-on:input="onInput"/>
  </div>
</template>

<script>
export default {
  props: ["value"],
  methods: {
    onInput(event) {
      this.$emit("input", event.target.value);
    }
  }
};
</script>

<style scoped>
</style>
