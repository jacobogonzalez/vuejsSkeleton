
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
  <div class="flex">
    <Card />
  </div>
</template>


<style scoped></style>
