<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>Vuetify</span>
        <span class="font-weight-light">MATERIAL DESIGN</span>
      </v-toolbar-title>
    </v-toolbar>

    <v-content>
      <ScrollSample/>
    </v-content>
  </v-app>
</template>

<script>
import ScrollSample from './components/ScrollSample'

export default {
  name: 'App',
  components: {
    ScrollSample
  },
  data () {
    return {
      //
    }
  }
}
</script>
