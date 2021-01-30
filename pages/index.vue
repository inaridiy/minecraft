<template>
  <v-main>
    <div class="relative ">
      <HomeImages />
      <div class="title absolute top-2/4 left-2/4 text-gray-50 rounded-lg">
        <h1 class="text-8xl  ">無名サーバー</h1>
        <p class="text-1xl text-center">キャッチフレーズ募集中</p>
      </div>
    </div>
    <v-container> <HomeMenu /></v-container>
  </v-main>
</template>

<script></script>

<style scoped>
.title {
  transform: translate(-50%, -50%);
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
