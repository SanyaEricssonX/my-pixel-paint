<template>
  <div class="config">
    <div class="config-left">
      <span class="config__desc">Введите размер холста:</span>
      Ширина:
      <div class="config__input">
        <pp-input type="number" v-model="input.x" /> px
      </div>
      Длина:
      <div class="config__input">
        <pp-input type="number" v-model="input.y" /> px
      </div>
    </div>
    <div class="config-right">
      <pp-button>Создать холст</pp-button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      input: {
        x: "",
        y: "",
      },
    };
  },
};
</script>

<style scoped>
.config {
  display: flex;
  /* justify-content: space-between; */
  width: 500px;
  border: 1px solid white;
  padding: 15px;
}
.config-left {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 50%;
}
.config__desc {
  margin-bottom: 15px;
}
.config__input {
  margin-top: 5px;
}
.config__input:not(:last-child) {
  margin-bottom: 5px;
}
.config-right {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 50%;
}
</style>