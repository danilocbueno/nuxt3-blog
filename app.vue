<template>
  <div class="sm:py-10">
    <Html lang="pt-br" />
    <Meta property="og:image" content="/cover.jpg" />
    <Meta name="twitter:card" content="summary_large_image" />
    <Navbar />

    <div class="max-w-6xl px-4 py-10 m-auto bg-white sm:px-8 sm:shadow dark:bg-gray-800 sm:rounded dark:text-gray-200">
      <NuxtPage />
    </div>

    <footer>
      rodape
      <button class="py-2 px-3 bg-indigo-500 text-white text-sm font-semibold rounded-md shadow focus:outline-none hover:bg-sky-700">
        botao teste
      </button>
    </footer>
  </div>
</template>

<style lang="postcss">
body {
  /* @apply bg-gray-50 dark:bg-gray-900; */
}
</style>
