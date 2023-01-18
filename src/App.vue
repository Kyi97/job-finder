<template>
  <v-app style="background-color: #faf8f4">
    <AppBar />
    <v-main>
      <v-divider style="margin-top: 4rem"></v-divider>
      <HomeView />
      <CategoriesView />
      <AccountView />
    </v-main>
  </v-app>
</template>

<script>
import AppBar from "./components/AppBar.vue";
import HomeView from "./views/HomeView.vue";
import CategoriesView from "./components/CategoriesSection.vue";
import AccountView from "./components/AccountSection.vue";

export default {
  name: "App",
  components: {
    AppBar,
    HomeView,
    CategoriesView,
    AccountView,
  },

  data: () => ({
    //
  }),
};
</script>
<style scoped>
</style>
