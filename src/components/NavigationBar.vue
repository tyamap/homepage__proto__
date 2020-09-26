<template>
  <v-card height="224">
    <v-app-bar
      fixed
      color="indigo lighten-1"
      dark
      shrink-on-scroll
      prominent
      src="https://picsum.photos/1920/1080"
      fade-img-on-scroll
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(100,115,201,.7), rgba(25,32,72,.7)"
        ></v-img>
      </template>

      <v-spacer></v-spacer>
      <v-toolbar-title>Title</v-toolbar-title>

      <v-spacer></v-spacer>

      <template v-slot:extension>
        <v-tabs align-with-title fixed-tabs>
          <v-tab>message</v-tab>
          <v-tab>about</v-tab>
          <v-tab>works</v-tab>
          <v-tab>blog</v-tab>
          <v-tab>contact</v-tab>
        </v-tabs>
      </template>
    </v-app-bar>
    <v-sheet height="100%"></v-sheet>
  </v-card>
</template>
