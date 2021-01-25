<template>
  <v-app>
    <v-main>
      <v-container fill-height fluid class="test2">
        <router-view/>
      </v-container>
    </v-main>
  </v-app>
</template>

<style>
.test2{
  background-image: url("assets/happy2_updated.jpg");
  background:linear-gradient(0deg, rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0.75)), url("assets/happy2_updated.jpg");
  background-size:cover;
}
</style>
