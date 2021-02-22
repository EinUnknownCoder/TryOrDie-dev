<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12"> </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">Try or Die!</h1>
      </v-col>

      <v-col class="mb-5" cols="12">
        <v-btn @click="roll" color="primary" x-large>Dreh das Rad!</v-btn>
      </v-col>

      <v-col class="mb-5" cols="12">
        <h2>{{ result.title }}</h2>
      </v-col>

      <v-col class="mb-5" cols="12">
        <h3>{{ result.text }}</h3>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "HelloWorld",

  methods: {
    roll() {
      console.log(Math.floor(Math.random() * 24));
      this.result = this.arr[Math.floor(Math.random() * 24)]
    },
  },

  data: () => ({
    result: {title: "Noch nicht gedreht", text: "Dreh bitte am Rad!"},
    arr: [ // 24 Segmente
      {title: "Trinken: 1", text: "Trink den Inhalt des Bechers!"},
      {title: "Trinken: 2", text: "Trink den Inhalt des Bechers!"},
      {title: "Trinken: 3", text: "Trink den Inhalt des Bechers!"},
      {title: "Trinken: 4", text: "Trink den Inhalt des Bechers!"},
      {title: "Trinken: 5", text: "Trink den Inhalt des Bechers!"},
      {title: "Trinken: 6", text: "Trink den Inhalt des Bechers!"},
      {title: "Mixen: 1", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 1", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 2", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 2", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 3", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 3", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 4", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 4", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 5", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 5", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 6", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Mixen: 6", text: "Nimm den Becher und fülle ihn in irgendein Becher.\nIst der Becher aber schon randvoll, musst du ihn trinken.\nHast du keinen weiteren Becher zum Umfüllen, musst du den Becher trinken!"},
      {title: "Prosten!", text: "Wähle einen Mitspieler und einen Becher aus.\nDieser muss den Becher trinken.\nDieser führt das Gleiche mit dir aus!"},
      {title: "Prosten!", text: "Wähle einen Mitspieler und einen Becher aus.\nDieser muss den Becher trinken.\nDieser führt das Gleiche mit dir aus!"},
      {title: "Wählen!", text: "Wähle einen Spieler.\nDer muss ein Becher seiner Wahl trinken!"},
      {title: "Wählen!", text: "Wähle einen Spieler.\nDer muss ein Becher seiner Wahl trinken!"},
      {title: "Klauen!", text: "Klaue einen Chip von einem deiner Mitspieler!"},
      {title: "Pleite!", text: "Du verlierst alle deine Chips!"},
    ]
  }),
};
</script>
