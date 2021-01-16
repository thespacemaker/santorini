<template>
        <v-row align="center" justify="center" class="container px-8">
            <v-col class="border ma-8" cols="12">
              <Banner />
              <HelloWorld />
              <v-btn class="text-center">Contact Us</v-btn>
            </v-col>
          </v-row>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Banner from '@/components/Banner.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Banner
  }
}
</script>

<style>
.border {
  border: 5px solid white;
  /* background-color: red; */
}
.container {
  height:"200";
  /* background-color: green; */
}
</style>
