<template>
  <div class="about">
    <div class="ml-10 lg:ml-28">
      <a id="about" class="lg:ml-20"><h1 class="text-3xl font-bold mb-6 ">Sobre mí</h1></a>
    </div>

    <section
      class="
        flex flex-col
        lg:flex-row lg:items-center
        justify-center
        w-4/5
        lg:w-4/5
        mx-auto
        lg:gap-8
      "
    >
      <div class="lg:max-w-xl lg:mr-12">
        <h3 class="text-2xl font-bold mb-4 lg:mr-36">Perfil</h3>
        <p class="mb-8">
          Soy <strong class="text-blue">Front-end Developer</strong> y
          bachiller en
          <strong class="text-blue">Administración y Marketing</strong>.<br>
          Mi creatividad y mi curiosidad me han llevado a explorar cosas nuevas y a
          educarme constantemente. Esto me acercó al diseño y luego a la tecnología,
          especificamente al mundo del desarrollo web. <br>
          Siempre me dio curiosidad saber cómo se construía una página web, saber cómo
          lograban implementar el diseño y además darle funcionalidad. Fue así como apareció
          el bichito de querer saber más, así que ni bien entré a este mundo, no di vuelta
          atrás.<br>
          Ahora soy recién egresada del <strong>Bootcamp de
          <u class="text-blue"><a href="https://www.laboratoria.la/" target="_blank">Laboratoria</a></u></strong>,
          donde pude desenvolverme por 6 meses en un espacio que simulaba un ambiente laboral.
          Aquí pude aprender desarrollo web en base a proyectos, utilizando
          la <strong>metodología SCRUM</strong>.<br>
          Lo que más me motiva, es la idea de poder desarrollar soluciones digitales
          que generen valor a las marcas y conecten con las personas.
        </p>
      </div>

      <div>
        <div
          class="bg-gray-100 flex items-center justify-center
          lg:w-auto"
        >
          <div class="container max-w-screen-lg mx-auto">
            <div>
              <h3 class="text-2xl font-bold mb-6">Habilidades</h3>
              <button
                v-for="icon in icons"
                v-bind:key="icon.name"
                class="inline-flex items-center space-x-2 rounded mr-6 mb-6 w-12"
              >
                <img :src="icon.url" alt="" />
              </button>
            </div>
          </div>
        </div>

        <div class="items">
          <h3 class="text-2xl font-bold mb-6">Intereses</h3>
          <div class="flex flex-wrap">
            <span
              v-for="item in items"
              class="px-4 py-2 bg-lightBlue font-normal mr-4 mb-4"
              v-bind:key="item"
              >{{ item }}</span
            >
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import html from '../assets/html.svg';
import css from '../assets/css.svg';
import js from '../assets/javascript.svg';
import git from '../assets/git.svg';
import github from '../assets/githubDark.svg';
import vue from '../assets/vue.svg';
import photoshop from '../assets/photoshop.svg';
import illustrator from '../assets/illustrator.svg';
import notion from '../assets/notion.svg';
import figma from '../assets/figma.svg';
import tailwind from '../assets/tailwind.svg';

export default {
  name: 'About',
  data() {
    return {
      items: [
        'Deportes',
        'Videojuegos',
        'Música',
        'Diseño',
        'Tecnología',
        'Branding',
        'Películas',
      ],
      icons: [
        {
          name: 'HTML',
          url: html,
          id: 'uno',
        },
        {
          name: 'CSS',
          url: css,
          id: 'dos',
        },
        {
          name: 'JavaScript',
          url: js,
          id: 'tres',
        },
        {
          name: 'Git',
          url: git,
          id: 'cuatro',
        },
        {
          name: 'Github',
          url: github,
          id: 'cinco',
        },
        {
          name: 'Vue.js',
          url: vue,
          id: 'seis',
        },
        {
          name: 'Photoshop',
          url: photoshop,
          id: 'siete',
        },
        {
          name: 'Illustrator',
          url: illustrator,
          id: 'ocho',
        },
        {
          name: 'Notion',
          url: notion,
          id: 'nueve',
        },
        {
          name: 'Figma',
          url: figma,
          id: 'diez',
        },
        {
          name: 'Tailwind',
          url: tailwind,
          id: 'once',
        },
      ],
    };
  },
};
</script>

<style scoped>
.items span {
  border-radius: 10px;
  border: solid 2px #2e5bff;
  color: #2e5bff;
}
</style>
