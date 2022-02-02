<template>
  <v-app>
    <Sidebar />
    <v-main>
      <v-container fluid class="main-container">
        <v-card ripple color="rgb(0,255,255)">
          <v-card-title>{{ page.title }}</v-card-title>
          <v-card-subtitle>{{ page.subtitle }}</v-card-subtitle>
        </v-card>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import Sidebar from "./components/sidebar/index.vue";

export default {
  name: "App",

  components: {
    Sidebar,
  },

  data: () => ({
    page: {
      title: "Welcome to the jungle",
      subtitle:
        "Aqui é aleatório, tem nada para ver. O que importa já está feito!",
    },
  }),
};
</script>
