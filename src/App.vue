<template>
  <v-app>
    <NavigationBar/>
    <v-main>
      <router-view></router-view>
    </v-main>
    <Footer/>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue';
import NavigationBar from './components/NavigationBar.vue';
import Footer from './components/Footer.vue';

export default Vue.extend({
  name: 'App',
  components:{
    NavigationBar,
    Footer,
  }
});
</script>
