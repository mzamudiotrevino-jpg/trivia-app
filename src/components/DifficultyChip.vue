<script setup>
const props = defineProps({
  difficulty: {
    type: String,
    required: true
  }
})
</script>

<template>
  <p
    class="px-5 py-2 rounded-full fixed uppercase text-white bottom-6 left-8 text-xl font-bold shadow-lg z-50"
    :class="props.difficulty === 'easy' ? 'bg-green-600' : props.difficulty === 'medium' ? 'bg-yellow-500' : 'bg-red-600'"
  >
    {{ props.difficulty }}
  </p>
</template>