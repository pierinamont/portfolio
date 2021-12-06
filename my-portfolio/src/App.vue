<template>
 <div>
    <div id="nav" class="flex justify-end pt-8">
      <router-link to="/" class="mr-8">Sobre mí</router-link>
      <router-link to="/" class="mr-8">Proyectos</router-link>
      <router-link to="/" class="mr-4 lg:mr-8">
        <span class="p-3 bg-blue hover:bg-blueDark">Contáctame</span>
      </router-link>
    </div>
  <router-view/>
 </div>
</template>

<style>
#app {
  font-family: 'Rubik', sans-serif;
}
span {
  color: white;
  border-radius: 10px;
}
</style>
