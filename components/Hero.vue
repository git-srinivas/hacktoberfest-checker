<template>
  <div class="z-0 w-full h-without-header">
    <div class="flex flex-col items-center justify-end text-center h-3/4">
      <div class="w-1/2">
        <h1 class="text-2xl Title md:text-4xl xl:text-6xl">
          Do they <strong>Hacktoberfest?</strong>
        </h1>
        <p class="Subtitle text-1xl md:text-2xl xl:text-3xl">
          Check if a project takes part in
          <strong>Hacktoberfest</strong> this year by looking up their
          repository URL.
        </p>
        <p class="mt-8">
          <NuxtLink to="checker" class="Button" @click.prevent="resetForm">
            Check a Repository
          </NuxtLink>
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.Title {
  @apply font-bold leading-none mb-4;
  color: var(--color-tertiary);
}

.Title strong {
  color: var(--color-secondary);
}

.Subtitle {
  @apply leading-tight tracking-wide;
  color: var(--color-tertiary);
}

.Subtitle strong {
  color: var(--color-secondary);
}

.Button {
  @apply px-8 rounded-lg w-1/4 py-3;
  background-color: var(--color-tertiary);
  color: var(--bg);
}

.Button:hover {
  background-color: var(--color-secondary);
}
</style>
