<template>
  <v-sheet dark id="contact" height="600" :color="colors[4]">
    <v-row class="fill-height" align="center" justify="center">
      <div class="display-3">{{ slides[4] }}</div>
    </v-row>
  </v-sheet>
</template>

<script lang="ts">
export default {
  data() {
    return {
      colors: [
        "indigo",
        "warning",
        "pink darken-2",
        "red lighten-1",
        "deep-purple accent-4",
      ],
      slides: ["Message", "About", "Works", "Blog", "Contact"],
    };
  },
};
</script>
