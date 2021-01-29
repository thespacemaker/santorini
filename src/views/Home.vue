<template>
  <v-row
    no-gutters
    style="flex-wrap: nowrap;"
    align="center"
    justify="center"
    class="container px-8 color"
  >
    <v-col v-if="form" cols="1" class="d-none d-lg-block mr-14"></v-col>
    <v-col class="border d-none d-lg-block flex-grow-1 flex-shrink-1" cols="12">
      <Banner />
      <div>
        <br>
        <h1 id="website" class="text-center d-none d-lg-block">
          New Website
        </h1>
        <h1 id="websiteMobile" class="text-center d-lg-none">
          New Website
        </h1>
        <h2 class="my-n4 mx-6 d-none d-lg-block text-center launching">
          LAUNCHING SOON!
        </h2>
        <h2 class="my-0 mx-6 d-lg-none text-center mobile">
          LAUNCHING SOON!
        </h2>
        <br>
        <h3 v-if="!form" class="text-center applying px-16 py-2">
          We are passionate about helping our clients overcome the difficult challenges they face with complex laws relating to...
        </h3>
        <v-row class="points py-3" align="center" justify="center">
          <v-col cols="3">
            <h3 class="mx-auto text-center">Immigration</h3>
          </v-col>
          <v-col cols="3">
            <h3 class="mx-auto text-center">Criminal Defense</h3>
          </v-col>
          <v-col cols="3">
            <h3 class="mx-auto text-center">Family Law</h3>
          </v-col>
        </v-row>
      </div>
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
        <Sidebar class="mr-16"/>
      </transition>
    </v-col>
  </v-row>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import HelloWorldMobile from '@/components/HelloWorldMobile.vue'
import Banner from '@/components/Banner.vue'
import Sidebar from '@/components/Sidebar.vue'

export default {
  name: 'Home',
  components: {
    // HelloWorld,
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
.color {
  height:100%
}
.container {
  height:"200";
}
.fill {
  background-color: #27052B;
  height: 100%;
}
#website{
  font-family: Georgia;
  font-size: 4em;
  font-weight: normal;
}

#websiteMobile{
  font-family: Georgia;
  font-size: 2em;
  font-weight: normal;
}

.launching{
  font-family: Georgia;
  font-size: 4.5em;
  font-weight: bold;
  line-height: 1.2;
}

.mobile{
  font-family: Georgia;
  font-size: 2.3em;
  font-weight: bold;
}

.applying{
  font-family: Georgia;
  font-size: 2em;
  font-weight: normal;
}

.points{
  font-family: Georgia;
  font-size: 1.6em;
}
</style>
