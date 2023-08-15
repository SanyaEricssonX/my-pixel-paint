<template>
  <input class="input" :value="modelValue" @input="updateInput" />
</template>

<script>
export default {
  name: "pp-input",
  props: {
    modelValue: [String, Number],
  },
  methods: {
    updateInput(event) {
      this.$emit("update:modelValue", event.target.value);
    },
  },
};
</script>

<style scoped>
.input {
  border: 2px solid var(--main-color);
  padding: 5px 7px;
  width: 80px;
}
</style>