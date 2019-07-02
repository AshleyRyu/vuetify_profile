<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase">
        <span><a herf="@Home">Ashley</a></span>
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
    <v-footer
      height="auto"
      color="primary lighten-1"
    >
      <v-layout
        justify-center
        row
        wrap
      >
        <v-btn
          v-for="link in links"
          :key="link"
          color="white"
          flat
          round
        >
          {{ link }}
        </v-btn>
        <v-flex
          primary
          lighten-2
          py-3
          text-xs-center
          white--text
          xs12
        >
          &copy;2019 — <strong>copyright 2019 Ashley Ryu All Rights Reserved.</strong>
        </v-flex>
      </v-layout>
    </v-footer>
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
    links: [
        'Home',
        'About Us',
        'Team',
        'Services',
        'Blog',
        'Contact Us'
      ]
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
