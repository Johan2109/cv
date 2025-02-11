<template>
  <section class="mt-9 px-4 max-w-6xl mx-auto">
    <article
      class="border shadow-md rounded-xl flex flex-col md:flex-row bg-white dark:bg-gray-900"
    >
      <!-- Backend -->
      <div
        class="p-4 sm:p-6 md:border-r border-gray-300 dark:border-gray-700 w-full md:w-1/2"
      >
        <header>
          <p class="text-2xl sm:text-3xl font-bold text-red-600 text-center">
            Backend
          </p>
        </header>
        <p
          class="mt-2 text-base sm:text-lg text-gray-700 dark:text-gray-300 text-center"
        >
          Conocimientos de servicios escalables con mejores prácticas de
          desarrollo.
        </p>
        <footer class="mt-4 flex flex-wrap justify-center gap-2">
          <span class="c_pill">PHP</span>
          <span class="c_pill">Laravel</span>
          <span class="c_pill">CodeIgniter</span>
          <span class="c_pill">PostgreSQL / MySQL / SQL</span>
          <span class="c_pill">Git / GitHub</span>
        </footer>
      </div>

      <!-- Frontend -->
      <div class="p-4 sm:p-6 w-full md:w-1/2">
        <header>
          <p class="text-2xl sm:text-3xl font-bold text-red-600 text-center">
            Frontend
          </p>
        </header>
        <p
          class="mt-2 text-base sm:text-lg text-gray-700 dark:text-gray-300 text-center"
        >
          Desarrollo de sitios web con una estructura de contenido simple,
          patrones de diseño limpios e interacciones bien pensadas.
        </p>
        <footer class="mt-4 flex flex-wrap justify-center gap-2">
          <span class="c_pill">JavaScript</span>
          <span class="c_pill">VueJS</span>
          <span class="c_pill">ReactJS</span>
          <span class="c_pill">Angular</span>
          <span class="c_pill">HTML5</span>
          <span class="c_pill">CSS</span>
          <span class="c_pill">TailwindCSS</span>
        </footer>
      </div>
    </article>
  </section>
</template>

<style scoped>
.c_pill {
  @apply bg-red-600 text-white px-3 py-1 text-xs sm:text-sm rounded-full font-medium;
}
</style>
