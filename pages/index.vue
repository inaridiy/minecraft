<template>
  <v-main>
    <div class="relative ">
      <HomeImages />
      <div class="title absolute top-2/4 left-2/4 text-gray-50 rounded-lg">
        <h1 class="text-4xl md:text-6xl lg:text-8xl ">無名サーバー</h1>
        <p class="text-xl md:text-2xl text-center">キャッチフレーズ募集中</p>
        <div class="text-xl text-center">接続アドレス: inarimc.ml</div>
      </div>
    </div>
    <v-container>
      <HomeMenu />

      <article class="prose p-8">
        <h1>無名サーバーとは</h1>
        <div>
          Raspberry Pi で建てっているマイクラ生活鯖<br />
          バックアップ等も万全でCoreProtectなどの荒らし対策プラグインなども入っているから安心して遊べます。
        </div>
      </article>
    </v-container>
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
