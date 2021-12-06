<template>
  <div class="max-w-2xl mx-auto">
    <div
      class="
        bg-white
        shadow-md
        rounded-lg
        w-64
        dark:bg-gray-800 dark:border-gray-700
      "
      v-for="card in cards"
      v-bind:key="card.id"
    >
      <img
        class="rounded-t-lg"
        :src="card.img"
        alt=""
      />
      <div class="p-5">
        <a href="#">
          <h5
            class="
              text-gray-900
              font-bold
              text-2xl
              tracking-tight
              mb-2
              dark:text-white
            "
          >
            {{card.title}}
          </h5>
        </a>
        <p class="font-normal text-gray-700 mb-3 dark:text-gray-400">
          {{card.description}}
        </p>
        <a
          href="#"
          class="
            text-white
            bg-blue-700
            hover:bg-blue-800
            focus:ring-4 focus:ring-blue-300
            font-medium
            rounded-lg
            text-sm
            px-3
            py-2
            text-center
            inline-flex
            items-center
            bg-blue
          "
        >
          Ver Proyecto
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import mdLinks from '../assets/mdLinks.svg';
import social from '../assets/socialNetwork.svg';
import dataLovers from '../assets/dataLovers.svg';
import cardValidation from '../assets/cardValidation.svg';

export default {
  name: 'Cards',
  data() {
    return {
      cards: [
        {
          id: 'uno',
          img: mdLinks,
          title: 'MdLinks',
          description:
            'Librería que permite validar links obtenidos de archivos markdown.',
        },
        {
          id: 'dos',
          img: social,
          title: 'Social Network',
          description:
            'Red Social que permita a los usuarios crear una cuenta de acceso y loguearse con ella; crear, editar, borrar y likear publicaciones.',
        },
        {
          id: 'tres',
          img: dataLovers,
          title: 'Data Lovers',
          description:
            'Interfaz web sobre el Studio Ghibli, donde se pueda visualizar y manipular data sobre sus películas.',
        },
        {
          id: 'cuatro',
          img: cardValidation,
          title: 'Card Validation',
          description:
            'Aplicación web que le permita a un usuario validar el número de una tarjeta de crédito. ',
        },
      ],
    };
  },
};
</script>
