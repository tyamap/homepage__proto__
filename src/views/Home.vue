<template>
  <div class="home">
    <Carousel/>
    <Message/>
    <About/>
    <Works/>
    <Blog/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Message from '@/components/Message.vue';
import Carousel from '@/components/Carousel.vue';
import About from '@/components/About.vue';
import Works from '@/components/Works.vue';
import Blog from '@/components/Blog.vue';

export default {
  components:{
    Carousel,
    Message, 
    About,
    Works,
    Blog,
  }
}
</script>
