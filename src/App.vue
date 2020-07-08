<template>
  <v-app>
    <AppHeader />
    <v-main>
      <HelloWorld />
    </v-main>
  </v-app>
</template>

<script>
import AppHeader from "./components/AppHeader"
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",

  components: {
    HelloWorld,
    AppHeader
  },

  data: () => ({
    //
  })
};
</script>
