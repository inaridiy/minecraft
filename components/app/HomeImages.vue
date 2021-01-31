<template>
  <v-carousel cycle hide-delimiters :height="h" class="blur">
    <v-carousel-item
      class="blur"
      v-for="(image, i) in images"
      :key="i"
      :src="image"
    ></v-carousel-item>
  </v-carousel>
</template>
<style scoped>
.blur::after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background-color: black;
  opacity: 0.2;
  display: block;
}
</style>
<script>
export default {
  props: ["h"],
  data: () => ({
    imagenames: [
      "2021-01-06_10.58.16.jpg",
      "2021-01-06_15.49.06.jpg",
      "2021-01-24_23.12.15.jpg",
      "2021-01-29_21.49.50.jpg",
      "2021-01-29_21.50.25.jpg",
      "2021-01-29_21.50.49.jpg",
      "2021-01-29_21.51.45.jpg",
      "2021-01-29_21.51.58.jpg",
      "2021-01-29_21.52.09.jpg",
      "2021-01-29_21.52.15.jpg",
      "2021-01-29_21.52.30.jpg",
      "2021-01-29_21.53.00.jpg",
      "2021-01-29_21.53.12.jpg",
      "2021-01-29_21.53.30.jpg",
      "2021-01-29_21.53.50.jpg",
      "2021-01-29_21.56.11.jpg",
      "2021-01-29_21.56.44.jpg",
      "cc6d4c69a80c0503.jpg",
      "image0.jpg",
      "11f750f802b18a44.jpg"
    ]
  }),
  computed: {
    images: function() {
      return this.imagenames.map(ele => `/images/minecraft/${ele}`);
    }
  }
};
</script>
