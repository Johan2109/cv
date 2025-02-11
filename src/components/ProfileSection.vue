<template>
  <main
    class="mt-4 sm:mt-6 lg:mt-8 xl:mt-10 mx-auto w-full px-8 rounded-xl py-8"
  >
    <div class="flex flex-col lg:flex-row items-center lg:items-stretch w-full">
      <div
        class="relative w-full lg:w-[50%] flex justify-center lg:justify-start"
      >
        <img
          :src="isMobile ? fotoMovil : fotoDesktop"
          alt="Foto de perfil"
          class="transition-all duration-300 w-[40%] sm:w-[35%] md:w-[30%] lg:w-full h-auto rounded-full lg:rounded-r-xl"
        />
      </div>

      <div
        class="lg:w-[60%] text-center lg:text-left flex flex-col justify-center px-8 lg:px-10"
      >
        <h1
          class="text-3xl font-extrabold text-gray-900 sm:text-4xl md:text-5xl lg:text-6xl"
        >
          <span
            class="bg-gradient-to-r from-red-600 to-red-400 bg-clip-text text-transparent"
          >
            Johan López Montes
          </span>
        </h1>

        <p class="mt-3 text-lg text-gray-600 sm:text-xl md:text-2xl">
          Ingeniero de software | Desarrollador FullStack
        </p>

        <p class="mt-2 text-base text-gray-500 sm:text-lg md:text-xl">
          JavaScript | VueJS | ReactJS | PHP | Laravel | CodeIgniter | HTML5 |
          CSS | TailwindCSS | PostgreSQL | MySQL | Git | GitHub | Linux | API
          REST | Scrum y Metodologías ágiles.
        </p>

        <p class="mt-2 text-sm text-gray-500 sm:mt-4 sm:text-base md:text-lg">
          Dispuesto a cumplir con las distintas funciones amando lo que hago.
        </p>

        <p class="mt-2 text-sm text-gray-500 sm:mt-4 sm:text-base md:text-lg">
          Desde hace 7 años trabajo en el mundo del desarrollo web, soy una
          persona joven, proactiva, con la capacidad de trabajo en equipo,
          comprometido, serio, dinámico y responsable con mis actividades de
          trabajo, con aspiraciones, deseos y metas basadas en el logro de
          objetivos, aprendo con rapidez y me intereso por cumplir de manera
          adecuada con puntualidad, honestidad y responsabilidad en las
          distintas actividades que realizo.
        </p>
      </div>
    </div>
  </main>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";
import fotoDesktop from "./../assets/foto1.jpeg";
import fotoMovil from "./../assets/foto2.png";

// Detectar si es móvil
const isMobile = ref(window.innerWidth < 1024);

const updateScreenSize = () => {
  isMobile.value = window.innerWidth < 1024;
};

onMounted(() => {
  window.addEventListener("resize", updateScreenSize);
});

onUnmounted(() => {
  window.removeEventListener("resize", updateScreenSize);
});
</script>
