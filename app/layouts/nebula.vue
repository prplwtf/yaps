<template>
  <div class="flex min-h-screen flex-col bg-nebula-slate-950">
    <NebulaNavigationbar />
    <div class="container grow space-y-12 self-center py-12">
      <slot />
    </div>
  </div>
</template>

<style>
@reference '~/assets/css/main.css'

* {
  @apply font-inter;
}

h1,
h2,
h3,
.display {
  @apply font-poppins;
}
</style>
