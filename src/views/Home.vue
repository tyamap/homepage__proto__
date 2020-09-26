<template>
  <div class="home">
    <Carousel/>
    <Message/>
    <About/>
    <Works/>
    <Blog/>
    <Contact/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Message from '@/components/Message.vue';
import Carousel from '@/components/Carousel.vue';
import About from '@/components/About.vue';
import Works from '@/components/Works.vue';
import Blog from '@/components/Blog.vue';
import Contact from '@/components/Contact.vue';

export default {
  components:{
    Carousel,
    Message, 
    About,
    Works,
    Blog,
    Contact,
  }
}
</script>
