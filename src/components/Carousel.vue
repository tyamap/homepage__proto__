<template>
  <v-carousel cycle height="calc(100vh - 224px)" hide-delimiter-background show-arrows-on-hover>
    <v-carousel-item v-for="slide in contents" :key="slide.id" :to="{hash: `#${slide.id}`}">
      <v-sheet :color="slide.color" height="100%">
        <v-row class="fill-height" align="center" justify="center">
          <div class="display-3">{{ slide.name }}</div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<script lang="ts">
export default {
  props: ["contents"],
  data() {
    return {
      colors: [
        "indigo",
        "warning",
        "pink darken-2",
        "red lighten-1",
        "deep-purple accent-4",
      ],
      slides: ["message", "about", "works", "blog", "contact"],
    };
  },
};
</script>
