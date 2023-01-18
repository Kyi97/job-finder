<template>
  <div>
    <v-app-bar color="#FFFAA2" absolute flat>
      <div class="layout">
        <v-toolbar-title class="mr-2">
          <img src="../assets/mlogo.png" alt="Logo" class="mr-2" height="48" />
        </v-toolbar-title>
        <v-spacer />
        <v-toolbar-items class="d-flex align-center">
          <v-layout row wrap>
            <v-toolbar-title
              v-for="title in titles"
              :key="title"
              color="#CAC9C5"
              class="text-bold ml-15 hidden-xs-only"
              >{{ title }}</v-toolbar-title
            >
          </v-layout>
        </v-toolbar-items>
        <v-spacer />
        <v-btn text @click="signIn" class="hidden-xs-only mt-3">Register</v-btn>
        <v-btn outlined @click="signIn" class="hidden-xs-only mt-3"
          >Sign In</v-btn
        >

        <v-menu
          v-model="menu"
          :close-on-content-click="false"
          :nudge-right="40"
        >
          <template v-slot:activator="{ on }">
            <v-btn icon v-on="on" class="hidden-sm-and-up" @click="menu = true">
              <v-icon>mdi-dots-vertical</v-icon>
            </v-btn>
          </template>
          <v-list class="justify-end">
            <v-list-item v-for="title in titles" :key="title">
              <v-list-item-title>{{ title }}</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
      </div>
    </v-app-bar>
  </div>
</template>
  
  
<script>
export default {
  name: "AppBar",
  data: () => ({
    titles: ["Home", "Pages", "Jobs", "Blog"],
    menu: false,
  }),
  methods: {
    signIn() {},
  },
};
</script>
<style scoped>
.text-bold {
  font-weight: 350;
}

.layout {
  margin-left: 5rem;
  margin-right: 5rem;
}
</style>