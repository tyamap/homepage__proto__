<template>
  <v-sheet dark :id="content.id" height="100vh" :color="content.color">
      <div class="display-3">{{ content.name }}</div>
  </v-sheet>
</template>

<script lang="ts">
export default {
  props:['content'],
};
</script>
