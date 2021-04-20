<template>
  <v-container>
    <v-row class="mb-6">
      <v-col v-for="n in 24" :key="n" xs="12" sm="6" md="4" xl="3">
        <v-card elevation="2" height="200"></v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  asyncData({ $config }) {
    return {
      data: $config.gsaoAuthClientSecret,
    }
  },
  methods: {
    test() {},
  },
}
</script>
