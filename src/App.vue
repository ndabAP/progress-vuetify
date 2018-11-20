<template>
  <div id="app">
    <v-app>
      <v-btn @click="toggle">Toggle</v-btn>

      <v-progress-circular
        v-if="isVisibleProgress"
        indeterminate
        color="green">
      </v-progress-circular>
    </v-app>
  </div>
</template>

<script>
export default {
  data: () => ({
    isVisibleProgress: false
  }),

  methods: {
    toggle () {
      this.isVisibleProgress = !this.isVisibleProgress
    }
  }
}
</script>
