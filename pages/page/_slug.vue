<template
  ><v-main
    ><HomeImages h="300" />
    <v-container
      ><article class="prose  w-full max-w-none">
        <h1 class="text-center">{{ page.title }}</h1>
        <nuxt-content :document="page" /></article
    ></v-container>
  </v-main>
</template>
<script>
export default {
  async asyncData({ $content, params }) {
    const page = await $content("pages", params.slug).fetch();

    return {
      page
    };
  }
};
</script>
