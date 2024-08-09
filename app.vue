<script setup lang="ts">
import SignaturePad from "signature_pad";

const canvas = ref();

onMounted(async () => {
  new SignaturePad(canvas.value);
});
</script>

<template>
  <div>
    <canvas ref="canvas"></canvas>
  </div>
</template>
