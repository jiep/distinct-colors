<script setup lang="ts">
defineProps<{ colors: Array<string> }>()
</script>

<template>
  <section class="container sm:mx-auto p-8 grid lg:grid-cols-6 grid-cols-2 gap-x-12 gap-y-8">
    <div class="rounded-lg text-center border flex flex-row items-center" v-for="color in colors">
      <span class="shrink-0 rounded-l-lg w-1/5 h-12" :style="{backgroundColor: color}"></span>
      <span class="shrink px-2 w-full text-gray-500 tabular-nums text-center select-all">{{ color }}</span>
      <span class="shrink-0 rounded-r-lg w-1/5 h-12" :style="{backgroundColor: color}"></span>
    </div>
  </section>
</template>
