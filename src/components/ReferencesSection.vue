<template>
  <section class="mt-9 px-4 max-w-4xl mx-auto">
    <h2
      class="text-4xl md:text-5xl font-extrabold bg-gradient-to-r from-red-600 to-red-400 bg-clip-text text-transparent text-center mb-6"
    >
      Referencias Laborales
    </h2>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
      <div
        v-for="referencia in referencias"
        :key="referencia.nombre"
        class="bg-white dark:bg-gray-900 shadow-md rounded-lg p-4 text-center"
      >
        <p class="text-lg font-semibold text-gray-900 dark:text-white">
          {{ referencia.nombre }}
        </p>
        <p class="text-gray-700 dark:text-gray-300">
          {{ referencia.cargo }}
        </p>
        <p class="text-gray-500 dark:text-gray-400">
          {{ referencia.telefono }}
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      referencias: [
        {
          nombre: "Santiago Espitia Patiño",
          cargo: "Ingeniero de Software",
          telefono: "+57 3508108761",
        },
        {
          nombre: "Luis Fernando Bello",
          cargo: "Ingeniero de Software",
          telefono: "+57 3003387000",
        },
        {
          nombre: "Wilson Fernando Suarez",
          cargo: "Ingeniero de Software",
          telefono: "+57 3012610193",
        },
        {
          nombre: "Jefferson Ayrton López Montes",
          cargo: "Ingeniero de Sistemas",
          telefono: "+57 3108564998",
        },
      ],
    };
  },
};
</script>
