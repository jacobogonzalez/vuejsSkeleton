
<script setup  lang="ts">
import { createApp } from 'vue';
import Card from './cards/card.vue'
createApp({
	components: {
		Card
	}
})
</script>
<template>
  <div class="d-flex pa-4">
    <v-container
      class="mx-0"
    >
      <v-row
        align="start"
        no-gutters
      >
        <v-col
        class="mx-2 my-2"
          v-for="n in 6"
          :key="n"
        >
        <Card />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>


<style scoped></style>
