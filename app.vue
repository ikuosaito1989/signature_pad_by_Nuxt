<script setup lang="ts">
import SignaturePad from "signature_pad";

const canvas = ref<HTMLCanvasElement>({} as HTMLCanvasElement);

onMounted(async () => {
  canvas.value.width = 600;
  canvas.value.height = 300;
  new SignaturePad(canvas.value, {
    backgroundColor: "rgba(255,255,255)",
  });
});
</script>

<template>
  <div class="bg-slate-100 h-svh flex">
    <canvas class="m-auto" ref="canvas"></canvas>
  </div>
</template>
