<template>
  <div
      class="relative flex items-top justify-center min-h-screen bg-gray-100 sm:items-center sm:pt-0"
  >
    <div class="max-w-4xl mx-auto sm:px-6 lg:px-8">
      <div class="bg-white overflow-hidden shadow sm:rounded-lg p-6 flex flex-col gap-4">
        <h2 class="text-2xl leading-7 font-semibold">
          Hello Flare!
        </h2>
        <p class="mt-3 text-gray-600 max-w-sm">
          Use this button to crash this nuxt@3 app and send a report to flare.
        </p>
        <button
            class="bg-emerald-500 rounded-md border-2 border-emerald-800/40 text-white uppercase tracking-wide px-4 py-2"
            @click="crash()"
        >
          crash
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NuxtTutorial',
  methods: {
    crash() {
      throw new Error('Error from Nuxt@3');
    }
  }
}
</script>
