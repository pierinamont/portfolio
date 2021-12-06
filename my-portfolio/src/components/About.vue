<template>
  <div class="about">
    <h1 class="text-3xl font-bold">Sobre mí</h1>

    <section class="flex flex-col lg:flex-row">
      <div class="mr-6">
          <p>It is a long established fact that a reader will be distracted by the
      readable content of a page when looking at its layout. The point of using
      Lorem Ipsum is that it has a more-or-less normal distribution of letters,
      as opposed to using 'Content here, content here', making it look like
      readable English. Many desktop publishing packages and web page editors
      now use Lorem Ipsum as their default model text, and a search for 'lorem
      ipsum' will uncover many web sites still in their infancy.</p>
      </div>

      <div>
         <div class="flex flex-col">
            <h3>Habilidades</h3>
            <div class="flex text-center">
              <span v-for="icon in icons" v-bind:key="icon.name" >
                <img :src="icon.url" alt=""/>
                {{icon.name}}
              </span>
            </div>
          </div>

        <div>
          <h3>Intereses</h3>
          <span v-for="item in items" class="p-3 bg-lightBlue" v-bind:key="item">{{item}}</span>
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
      items: ['Deportes', 'Videojuegos', 'Música', 'Diseño', 'Tecnología', 'Branding', 'Películas'],
      icons: [
        {
          name: 'HTML',
          url: html,
        },
        {
          name: 'CSS',
          url: css,
        },
        {
          name: 'JavaScript',
          url: js,
        },
        {
          name: 'Git',
          url: git,
        },
        {
          name: 'Github',
          url: github,
        },
        {
          name: 'Vue.js',
          url: vue,
        },
        {
          name: 'Photoshop',
          url: photoshop,
        },
        {
          name: 'Illustrator',
          url: illustrator,
        },
        {
          name: 'Notion',
          url: notion,
        },
        {
          name: 'Figma',
          url: figma,
        },
        {
          name: 'Tailwind',
          url: tailwind,
        },
      ],
    };
  },
};
</script>
