<script setup>
const { path } = useRoute();
const { data } = await useAsyncData("content", () =>
  queryContent(path).only(["_path", "title"]).find()
);
</script>
<template>
  <main>
    <div v-for="link of data" :key="link._path">
      <NuxtLink :to="link._path">{{ link.title }}</NuxtLink>
    </div>

    <pre>
    {{ path }}
  </pre
    >

    <pre>
    {{ data }}
  </pre
    >
  </main>
</template>