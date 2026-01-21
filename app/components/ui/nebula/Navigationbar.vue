<template>
  <nav class="sticky top-0 left-0">
    <div class="flex flex-col items-center bg-slate-900 px-2 py-3 text-white">
      <div class="container py-0.5">
        <div class="flex items-center justify-between">
          <div class="flex items-center gap-2.5">
            <Icon name="bi:exclude" :size="40" mode="svg" />
            <div class="flex flex-col">
              <NuxtLink to="/" class="text-link block text-xs text-white!">
                prpl.wtf
              </NuxtLink>
              <span class="text-3xl font-bold">Nebula</span>
            </div>
          </div>
          <div class="flex items-center gap-2.5">
            <button
              class="flex items-center gap-1 rounded-lg bg-linear-to-r from-purple-400 to-blue-500 px-3 py-1 text-lg font-medium"
            >
              Try for free
              <Icon name="bi:arrow-right" :size="22" />
            </button>
          </div>
        </div>
      </div>
    </div>
    <div
      class="relative top-0 h-px w-full bg-linear-to-r from-slate-800 via-slate-500 to-slate-800 transition-all duration-500 md:static"
    />
  </nav>
</template>
