<template>
  <div class="home">
    <Hero class="mt-20"/>
    <About class="mt-56"/>
    <Cards class="mt-56"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Hero from '@/components/Hero.vue';
import About from '../components/About.vue';
import Cards from '../components/Cards.vue';

export default {
  name: 'Home',
  components: {
    Hero,
    About,
    Cards,
  },
};
</script>
