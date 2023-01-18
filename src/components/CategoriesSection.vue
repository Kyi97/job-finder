<template>
  <div>
    <v-layout row wrap>
      <h2>Browse by Job Categories</h2>
      <v-spacer v-if="$vuetify.breakpoint.mdAndUp" />
      <v-btn color="black" class="white--text">Browse All</v-btn>
    </v-layout>
    <v-layout row wrap>
      <v-flex v-for="item in items" :key="item.id" xs12 md3>
        <v-card class="pt-2 mb-5 mt-5 ml-2">
          <v-img :src="item.image" width="70" height="70" class="ml-3"></v-img>
          <v-card-title>{{ item.title }}</v-card-title>
          <v-card-text>{{ item.description }}</v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
  </div>
</template>
<script>
export default {
  name: "CategoriesSection",
  data: () => ({
    items: [
      {
        image: "https://img.icons8.com/clouds/100/null/web.png",
        title: "UI/UX Design",
        description: "75+ Available Vacancy",
      },
      {
        image: "https://img.icons8.com/bubbles/100/null/commercial.png",
        title: "Digital Marketing",
        description: "75+ Available Vacancy",
      },
      {
        image: "https://img.icons8.com/clouds/100/null/imac-settings.png",
        title: "It & Software",
        description: "75+ Available Vacancy",
      },
      {
        image: "https://img.icons8.com/clouds/100/null/data-configuration.png",
        title: "Data Science",
        description: "75+ Available Vacancy",
      },
      {
        image: "https://img.icons8.com/clouds/100/null/monitor.png",
        title: "Computer Science",
        description: "75+ Available Vacancy",
      },
      {
        image: "https://img.icons8.com/clouds/100/null/code.png",
        title: "Web Development",
        description: "75+ Available Vacancy",
      },
      {
        image: "https://img.icons8.com/clouds/100/null/training.png",
        title: "Project Management",
        description: "75+ Available Vacancy",
      },
      {
        image: "https://img.icons8.com/clouds/100/null/more.png",
        title: "Jobs are waiting for you",
        description: "Explore More",
      },
    ],
  }),
};
</script>