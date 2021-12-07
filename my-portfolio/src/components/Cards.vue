<template>
<div>
<a id="projects"><h1 class="text-3xl font-bold mb-6 lg:pr-36">Proyectos</h1></a>
  <div class=" mx-auto flex flex-wrap flex-row gap-5 justify-center">
    <div
      class="
        bg-white
        shadow-md
        rounded-lg
        w-64
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
              text-xl
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
        <div class="flex flex-col text-center">
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
                hover:bg-blueDark
                w-3/4
                m-auto
                justify-center
            "
            style="color: white"
            >
            Ver Proyecto
            </a>
            <a class="cursor-pointer text-blue" href="card.github">Ver repositorio</a>
        </div>
      </div>
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
            'Librería que permite validar links obtenidos de archivos markdown, obteniendo los links rotos, válidos, únicos y sus estados.',
          github: 'https://github.com/pierinamont/LIM015-md-links',
        },
        {
          id: 'dos',
          img: social,
          title: 'Social Network',
          description:
            'Red Social que permita a los usuarios crear una cuenta de acceso y loguearse con ella; crear, editar, borrar y likear publicaciones.',
          github: 'https://github.com/pierinamont/LIM015-social-network',
        },
        {
          id: 'tres',
          img: dataLovers,
          title: 'Data Lovers',
          description:
            'Interfaz web sobre el Studio Ghibli, donde se pueda visualizar y manipular data según las especificaciones de los usuarios.',
          github: 'https://github.com/pierinamont/LIM015-data-lovers',
        },
        {
          id: 'cuatro',
          img: cardValidation,
          title: 'Card Validation',
          description:
            'Aplicación web que le permite a los usuario validar el número de una tarjeta de crédito y ver a qué banco pertenece. ',
          github: 'https://github.com/pierinamont/LIM015-card-validation',
        },
      ],
    };
  },
};
</script>
