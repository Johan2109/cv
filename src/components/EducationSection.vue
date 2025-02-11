<template>
  <section class="mt-9 px-4 max-w-4xl mx-auto">
    <h2
      class="text-4xl md:text-5xl font-extrabold bg-gradient-to-r from-red-600 to-red-400 bg-clip-text text-transparent text-center mb-6"
    >
      Educación
    </h2>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
      <div
        v-for="estudio in educacion"
        :key="estudio.titulo"
        class="bg-white dark:bg-gray-900 shadow-md rounded-lg p-4 text-center"
      >
        <p class="text-lg font-semibold text-gray-900 dark:text-white">
          {{ estudio.titulo }}
        </p>
        <p class="text-gray-700 dark:text-gray-300">
          {{ estudio.institucion }}
        </p>
        <p class="text-gray-500 dark:text-gray-400">
          {{ estudio.anio }}
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      educacion: [
        {
          titulo: "Ingeniero de Software",
          institucion: "Fundación Universitaria Compensar",
          anio: "2022",
        },
        {
          titulo: "Técnico en Diseño Web",
          institucion: "Politécnico Grancolombiano",
          anio: "2015",
        },
        {
          titulo: "Bachillerato Académico",
          institucion: "Institución Educativa Distrital Justo Victor Charry",
          anio: "2015",
        },
      ],
    };
  },
};
</script>
