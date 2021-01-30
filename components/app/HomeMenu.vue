<template
  ><v-row>
    <v-col cols="12" sm="6" v-for="ele in menu" :key="ele.txt">
      <v-card
        ><v-card-title
          ><v-icon large>{{ ele.icon }}</v-icon> {{ ele.txt }}</v-card-title
        >
      </v-card>
    </v-col></v-row
  >
</template>
<script>
export default {
  data: function() {
    return {
      menu: [
        { icon: "mdi-ruler-square-compass", txt: "サーバールール" },
        { icon: "mdi-shield-check", txt: "サーバー利用規約" },
        { icon: "mdi-microsoft-xbox-controller", txt: "初めて入った方へ" },
        { icon: "mdi-calendar-month", txt: "イベント--Coming Sonn--" }
      ]
    };
  }
};
</script>
