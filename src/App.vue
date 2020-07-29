<template>
  <v-app>
    <AppBar></AppBar>
    <br>
    <br>
    <br>
    <v-container>
      <router-view></router-view>
    </v-container>
  </v-app>
</template>

<script>
import AppBar from './components/AppBar'

export default {
  name: 'App',

  components: {
    AppBar
  },

  data: () => ({
    //
  }),
};
</script>
