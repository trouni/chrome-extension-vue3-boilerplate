<template>
  <div
    class="flex fixed right-0 bottom-0 z-50 m-5 font-sans leading-none select-none"
  >
    <div
      class="w-max h-min text-gray-800 bg-white rounded-full shadow"
      p="x-4 y-2"
      m="y-auto r-2"
      transition="opacity duration-300"
      :class="show ? 'opacity-100' : 'opacity-0'"
    >
      Vitesse WebExt
    </div>
    <div
      class="flex w-10 h-10 rounded-full shadow cursor-pointer"
      bg="teal-600 hover:teal-700"
      @click="toggle()"
    >
      <pixelarticons-power class="block m-auto text-lg text-white" />
    </div>
  </div>
</template>

<script setup lang="ts">
import { useToggle } from '@vueuse/core'
import '~/styles'

const [show, toggle] = useToggle(false)
</script>
