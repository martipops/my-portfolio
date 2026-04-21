<template>
  <div class="project flex-col flex">
    <img :src="project.image" class="w-full object-cover rounded-md pb-4" />
    <h2 class="text-2xl font-bold! text-[#ffd60a] pb-2">{{ project.title }}</h2>
    <p class="text-sm text-[#d8f3dc]/70">{{ project.description }}</p>
  </div>
</template>

<script lang="ts">
import type { Projects } from '@/interfaces/projects';

export default {
  props: {
    project: {
      type: Object as () => Projects,
      required: true,
    }
  }
}
</script>
