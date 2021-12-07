<template>
 <div>
    <div id="nav" class="flex justify-end pt-8 font-semibold ">
      <a href="#about" class="mr-8">Sobre mí</a>
      <a href="#projects" class="mr-8">Proyectos</a>
      <a href="mailto:pierinamfatur@gmail.com" class="mr-4 lg:mr-8">
        <span class="p-3 bg-blue hover:bg-blueDark">Contáctame</span>
      </a>
    </div>
  <router-view/>
   <Footer/>
 </div>

</template>

<script>
import Footer from './components/Footer.vue';

export default {
  components: {
    Footer,
  },
};
</script>

<style scoped>
#app {
  font-family: 'Rubik', sans-serif;
}
span {
  color: white;
  border-radius: 10px;
}
</style>
