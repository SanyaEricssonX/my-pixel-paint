<template>
  <button class="btn">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "pp-button",
};
</script>

<style scoped>
.btn {
  padding: 10px 15px;
  font-weight: 900;
  font-size: 15px;
  border: none;
  border: 2px solid var(--main-color);
  color: var(--main-color);
  background-color: white;
  cursor: pointer;
  transition: background-color 0.3s ease, color 0.2s linear, border 1s ease;
}
.btn:hover {
  background-color: var(--main-color);
  color: white;
  border: 2px solid white;
}
.btn:active {
  transform: translateY(2px);
}
</style>