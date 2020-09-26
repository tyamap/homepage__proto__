<template>
  <div class="home">
    <Carousel :contents=contents />
    <HomeContent v-for="content in contents" :key="content.id" :content="content" />
  </div>
</template>

<script>
import Carousel from "@/components/Carousel.vue";
import HomeContent from "@/components/HomeContent.vue";

export default{
  data() {
    return {
      contents:[
        {
          id: 'message',
          name: 'message',
          color: 'indigo',
        },
        {
          id: 'about',
          name: 'about',
          color: 'warning',
        },
        {
          id: 'works',
          name: 'works',
          color: 'pink darken-2',
        },
        {
          id: 'blog',
          name: 'blog',
          color: 'red lighten-1',
        },
        {
          id: 'contact',
          name: 'contact',
          color: 'deep-purple accent-4',
        },
      ],
    };
  },
  components: {
    Carousel,
    HomeContent,
  },
};
</script>
