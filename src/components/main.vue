
<script setup lang="ts">
import Header from './header/header.vue'
</script>
<template>
  <v-card>
    <v-layout class="appBackground">
      <v-navigation-drawer>
        <v-list>
          <v-list-item prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg" title="Sandra Adams"
            subtitle="sandra_a88@gmailcom"></v-list-item>
        </v-list>

        <v-divider></v-divider>

        <v-list density="compact" nav>
          <v-list-item prepend-icon="mdi-folder" title="My Files" value="myfiles"></v-list-item>
          <v-list-item prepend-icon="mdi-account-multiple" title="Shared with me" value="shared"></v-list-item>
          <v-list-item prepend-icon="mdi-star" title="Starred" value="starred"></v-list-item>
        </v-list>
      </v-navigation-drawer>

      <v-main class="mainContainer">
        <!-- header component is global for all applications -->
        <Header />
        <!-- The application works by routes, add your components to the index file in the router folder -->
        <router-view></router-view>
      </v-main>
    </v-layout>
  </v-card>
</template>


<style scoped>
.appBackground {
  background: #F5F5F5;
}
.mainContainer{
  height: 100vh;
  overflow: auto;
}
</style>
