<template>
  <div class="app">
    <h1 class="app__heading">Pixel Paint</h1>
    <config-field></config-field>
  </div>
</template>

<script>
import ConfigField from "@/components/ConfigField";
import PaintField from "@/components/PaintField";

export default {
  components: {
    ConfigField,
    PaintField,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
:root {
  --main-color: orange;
}
:focus {
  outline: 3px solid white;
}
body {
  background-color: grey;
  font-family: "Oswald", sans-serif;
  color: white;
}
.app {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
.app__heading {
  margin-bottom: 15px;
  color: white;
}
</style>
