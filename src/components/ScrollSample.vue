<template>
  <v-container>
    <v-layout
        justify-center
        row
        wrap
    >
      <v-flex xs12>
        <v-btn @click="dialog = true">Show dialog</v-btn>
      </v-flex>

      <v-flex xs12 :key="i" v-for="i in sampleData">{{ i }}</v-flex>
    </v-layout>
    <v-dialog v-model="dialog">Dialog</v-dialog>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      dialog: false,
      sampleData: Array.apply(null, {length: 100}).map(Number.call, Number),
    }),
  }
</script>

<style>

</style>
