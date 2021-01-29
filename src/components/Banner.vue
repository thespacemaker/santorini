<template>
  <div>
    <v-row align="center" justify="center" class="text-center">
      <v-col class="d-none d-md-block" cols="4">
        <h2 class="bigger">SE HABLA ESPAÑOL!</h2>
      </v-col>
      <v-col class="d-md-none" cols="4">
      </v-col>
      <v-col cols="4" class="flex-grow-1 flex-shrink-0 d-none d-md-block pt-6">
        <v-img min-height="125" max-height="125" contain src="logo-white.png"></v-img>
      </v-col>
      <v-col cols="4" class="flex-grow-1 flex-shrink-0 pt-6 d-md-none">
        <v-img min-height="125" max-height="125" contain src="logo-white.png"></v-img>
      </v-col>
      <v-col class="d-none d-md-block" cols="4">
        <a class="phone" href="tel:+17138427390">
          <h2 class="bigger"><v-icon>mdi-phone</v-icon> 713-842-7390</h2>
        </a>
      </v-col>
      <v-col class="d-md-none" cols="4">
        <a class="phone" href="tel:+17138427390">
          <h2><v-icon>mdi-phone</v-icon></h2>
        </a>
      </v-col>
    </v-row>
  </div>
</template>

<script>
</script>

<style scoped>
.phone {
  color: white;
  text-decoration: none;
}

.bigger {
  font-size: 2em
}
</style>
