<template>
  <footer class="w-full bg-red-600 text-white py-4">
    <div
      class="max-w-4xl mx-auto w-full px-4 flex items-center justify-between gap-x-4 lg:gap-x-16"
    >
      <!-- Logo de LinkedIn con bordes y tamaño ajustado -->
      <a
        href="https://www.linkedin.com/in/tu-perfil"
        target="_blank"
        class="border-2 border-white text-white text-lg font-semibold px-8 py--5 rounded-full transition-all hover:bg-white hover:text-red-600 hover:shadow-lg"
      >
        <img
          src="@/assets/logo-linkedin.png"
          alt="LinkedIn"
          class="w-18 h-12 transition-all hover:scale-110"
        />
      </a>

      <!-- Botón de descarga de PDF -->
      <button
        @click="downloadPDF"
        class="border-2 border-white text-white text-lg font-semibold px-6 py-2 rounded-full transition-all hover:bg-white hover:text-red-600 hover:shadow-lg"
      >
        Descargar PDF
      </button>
    </div>
  </footer>
</template>

<script>
import html2pdf from "html2pdf.js";

export default {
  methods: {
    downloadPDF() {
      const element = document.body;
      html2pdf().from(element).save("hoja_de_vida.pdf");
    },
  },
};
</script>
