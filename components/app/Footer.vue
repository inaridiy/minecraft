<template>
  <v-footer dark>
    <v-row justify="center" no-gutters>
      <v-btn
        v-for="link in links"
        :key="link.txt"
        :href="link.link"
        color="white"
        text
        rounded
        class="my-2"
      >
        {{ link.txt }}
      </v-btn>
      <v-col class=" py-4 text-center white--text" cols="12">
        {{ new Date().getFullYear() }} — <strong>無名サーバー</strong>
      </v-col>
    </v-row>
  </v-footer>
</template>
<script>
export default {
  data: function() {
    return {
      links: [
        { txt: "サーバーマップ", link: "https://map.inarimc.ml/" },
        { txt: "主のTwitter", link: "https://twitter.com/inarizushi19" },
        { txt: "主のブログ", link: "https://inaridiy.tk/" }
      ]
    };
  }
};
</script>
