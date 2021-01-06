<template>
  <v-row align="center" justify="center" class="container px-8">
    <v-col class="border ma-8" cols="12">
      <v-card>

      </v-card>
      <HelloWorld />
    </v-col>
  </v-row>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style>
.border {
  border: 5px solid white;
  /* background-color: red; */
}
.container {
  height:"100";
  /* background-color: green; */
}
</style>
