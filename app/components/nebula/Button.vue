<template>
  <button
    v-if="props.variant == 'primary'"
    class="button bg-nebula-brand text-black hover:bg-nebula-slate-50"
    :class="props.class"
  >
    <slot />
  </button>

  <button
    v-if="props.variant == 'secondary'"
    class="button bg-nebula-slate-500 hover:bg-nebula-slate-400"
    :class="props.class"
  >
    <slot />
  </button>
</template>

<script setup lang="ts">
const props = withDefaults(
  defineProps<{
    class?: string
    variant?: 'primary' | 'secondary'
  }>(),
  {
    variant: 'secondary',
  }
)
</script>

<style scoped>
@reference '~/assets/css/main.css';

.button {
  @apply flex cursor-pointer items-center gap-1 rounded-full px-6 py-2 text-lg font-medium transition-colors;
}
</style>
