<template>
  <main class="py-10 px-4 text-center text-gray-700 dark:text-gray-200">
    <pixelarticons-sliders class="mx-2 text-2xl icon-btn" />
    <div>Options</div>
    <p class="mt-2 opacity-50">
      This is the options page
    </p>

    <input v-model="storageDemo" class="py-1 px-2 mt-2 rounded border border-gray-400">

    <div class="mt-4">
      Powered by Vite <pixelarticons-zap class="align-middle" />
    </div>
  </main>
</template>

<script setup lang="ts">
import { storageDemo } from '~/logic/storage'
</script>
