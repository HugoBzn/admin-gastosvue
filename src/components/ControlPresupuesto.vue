<script setup>
import imagen from "../assets/img/grafico.jpg";
</script>

<template>
  <div>
    <div class="dos-columnas">
      <div class="contenedor-grafico">
        <img :src="imagen" alt="imagen contenedor grafico" />
      </div>

      <div class="contenedor-presupuesto">
        <button class="reset-app">Resetar app</button>

        <p>
          <span>Presupuesto:</span>
          $0
        </p>
        <p>
          <span>Disponible:</span>
          $0
        </p>
        <p>
          <span>Gastado:</span>
          $0
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
