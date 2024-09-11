<template>
  <q-page class="flex flex-center">
    <img
      alt="Quasar logo"
      src="~assets/quasar-logo-vertical.svg"
      style="width: 200px; height: 200px"
    />
  </q-page>
</template>

<script setup>
import { useLocalStorage, useMouse, usePreferredDark } from "@vueuse/core";

const { x, y } = useMouse();

window.addEventListener("mousemove", () => {
  console.log("Coordenadas do Mouse: ", x.value, y.value);
});

defineOptions({
  name: "IndexPage",
});
</script>
