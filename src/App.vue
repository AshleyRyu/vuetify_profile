<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>Ashley</span>
        <span class="font-weight-light">Ryu</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        flat
        href="https://github.com/AshleyRyu"
        target="_blank"
      >
        <span class="mr-2">Gitub</span>
      </v-btn>
    </v-toolbar>

    <v-content>
      <router-view/>
      <!-- <HelloWorld/> -->
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import store from './store'

export default {
  name: 'App',
  store,
  components: {
    store
    // HelloWorld
  },
  data () {
    return {
      //
    }
  }
}
</script>

<style media="screen">
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
  }
</style>
