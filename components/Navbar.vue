<template>
  <div class="flex justify-between max-w-6xl px-4 py-4 mx-auto sm:px-8">
    <!-- Navigation -->
    <h1 class="font-extrabold text-transparent bg-clip-text text-orange-900">
      Fábrica de Software
    </h1>
    <pre>{{ navigation }}</pre>
    <div class="text-gray-700 dark:text-gray-200">
      <ContentNavigation v-slot="{ navigation }">
        <NuxtLink
          v-for="link of navigation"
          :key="link._path"
          :to="link._path"
          active-class="font-bold"
          class="mr-4"
        >
          {{ link.navTitle || link.title }}
        </NuxtLink>
      </ContentNavigation>
    </div>
    <!-- Social icons & Color Mode -->
    <div class="space-x-3 text-gray-500 transition">
      <a href="https://twitter.com/Atinux" title="Twitter" class="hover:text-gray-700 dark:hover:text-gray-300"><Icon name="fa-brands:twitter" /></a>
      <a href="https://github.com/Atinux/content-wind" title="GitHub" class="hover:text-gray-700 dark:hover:text-gray-300"><Icon name="fa-brands:github" /></a>
      <ColorModeSwitch class="hover:text-gray-700 dark:hover:text-gray-300" />
    </div>
  </div>
</template>
