<template>
  <v-app light>
    <nuxt />
    <v-bottom-navigation
      :value="activeIndex"
      grow
      background-color="primary"
      mandatory
    >
      <v-btn>
        <span>Les boissons</span>
        <v-icon>mdi-history</v-icon>
      </v-btn>
      <v-btn>
        <span>Vos produits</span>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
    </v-bottom-navigation>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    return {
      activeIndex: 1,
    }
  },
})
</script>

<style scoped>
  .v-btn--active {
    color: white;
  }
</style>
