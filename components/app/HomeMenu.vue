<template
  ><v-row>
    <v-col cols="12" sm="6" v-for="ele in menu" :key="ele.txt">
      <v-card :to="ele.link"
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
        { icon: "mdi-bullhorn", txt: "お知らせ" },
        { icon: "mdi-shield-check", txt: "サーバールール", link: "/page/rule" },
        {
          icon: "mdi-microsoft-xbox-controller",
          txt: "初めて入った方へ",
          link: "/page/first"
        },
        { icon: "mdi-calendar-month", txt: "イベント--Coming Sonn--" }
      ]
    };
  }
};
</script>
