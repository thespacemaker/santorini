<template>
  <v-row
    no-gutters
    style="flex-wrap: nowrap;"
    align="center"
    justify="center"
    class="container px-8 color"
  >
    <v-col class="border d-none d-lg-block ma-8 flex-grow-0 flex-shrink-1" cols="12">
      <Banner />
      <HelloWorld />
      <h2 class="text-center">
        <v-btn v-if="!form" dark @click="showForm" class="my-8">Contact Us</v-btn>
        <v-btn v-if="form" dark @click="showForm" class="my-8">back</v-btn>
      </h2>
    </v-col>
    <v-col v-if="!form" class="border ma-8 d-lg-none flex-grow-1 flex-shrink-1" cols="12">
      <Banner />
      <HelloWorldMobile />
      <h2 class="text-center">
        <v-btn v-if="!form" dark @click="showForm" class="my-6">Contact Us</v-btn>
        <v-btn v-if="form" dark @click="showForm" class="my-6">back</v-btn>
      </h2>
    </v-col>

      <v-col
        transition="slide-x-transition"
        cols="12"
        v-if="form"
        class="color fill mt-n12 mb-n16 d-lg-none"
      >
        <transition
          appear
          name="slide-x-transition"
        >
          <Sidebar/>
        </transition>
      </v-col>
      <v-col
        transition="slide-x-transition"
        cols="6"
        v-if="form"
        class="color fill mt-n12 mb-n16 d-none d-lg-block"
      >
      <transition
        appear
        name="slide-x-transition"
      >
        <Sidebar/>
      </transition>
    </v-col>
  </v-row>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import HelloWorldMobile from '@/components/HelloWorldMobile.vue'
import Banner from '@/components/Banner.vue'
import Sidebar from '@/components/Sidebar.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    HelloWorldMobile,
    Banner,
    Sidebar
  },
  data: () => ({
    form: false
  }),
  methods: {
    showForm() {
      this.form = !this.form
    }
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
.color {
  /* background-color: red; */
  height: 100%;
}
.fill {
  background-color: #27052B;
  height: 100%;
}
</style>
