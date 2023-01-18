<template>
  <v-app style="background-color: #faf8f4">
    <AppBar />
    <v-main class="layout">
      <v-divider style="margin-top: 4rem"></v-divider>
      <HomeView />
      <v-divider style="margin-top: 4rem; margin-bottom: 3rem"></v-divider>
      <CategoriesView />
    </v-main>
  </v-app>
</template>

<script>
import AppBar from "./components/AppBar.vue";
import HomeView from "./views/HomeView.vue";
import CategoriesView from "./components/CategoriesSection.vue";
export default {
  name: "App",
  components: {
    AppBar,
    HomeView,
    CategoriesView,
  },

  data: () => ({
    //
  }),
};
</script>
<style scoped>
.layout {
  margin-left: 5rem;
  margin-right: 5rem;
}
</style>
