<template>
  <v-sheet dark :id="content.id" height="100vh" :color="content.color">
    <v-row class="fill-height" align="center" justify="center">
      <div class="display-3">{{ content.name }}</div>
    </v-row>
  </v-sheet>
</template>

<script lang="ts">
export default {
  props:['content'],
};
</script>
