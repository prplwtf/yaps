<template>
  <nav class="sticky top-0 left-0">
    <div
      class="flex flex-col items-center border-b border-nebula-slate-600 bg-linear-to-r from-nebula-slate-900 via-nebula-slate-800 to-nebula-slate-900 px-2 text-white"
    >
      <div class="container px-6 py-3">
        <div class="flex items-center justify-between">
          <div class="flex items-center gap-2.5">
            <Icon name="bi:exclude" :size="40" mode="svg" />
            <div class="flex flex-col">
              <NuxtLink to="/" class="text-link block text-xs text-white!">
                prpl.wtf
              </NuxtLink>
              <span class="font-poppins text-3xl font-semibold">Nebula</span>
            </div>
          </div>
          <div class="flex items-center gap-2.5">
            <NebulaButton> Blog </NebulaButton>
            <NebulaButton> Documentation </NebulaButton>
            <NebulaButton variant="primary">
              Try for free
              <Icon name="bi:arrow-right" :size="22" />
            </NebulaButton>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>
