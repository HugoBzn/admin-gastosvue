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

<style scoped>
.dos-columnas {
  display: flex;
  flex-direction: column;
}

@media (min-width: 768px) {
  .dos-columnas {
    flex-direction: row;
    gap: 4rem;
    align-items: center;
  }

  .dos-columnas > :first-child {
    margin-bottom: 0;
  }
}

.reset-app {
  background-color: #db2777;
  border: none;
  padding: 1rem;
  width: 100%;
  color: var(--blanco);
  font-weight: 900;
  text-transform: uppercase;
  border-radius: 1rem;
  transition-property: background-color;
  transition-duration: 300ms;
}

.reset-app:hover {
  cursor: pointer;
  background-color: #c11d67;
}

.contenedor-presupuesto {
  width: 100%;
}

.contenedor-presupuesto p {
  font-size: 2.4rem;
  text-align: center;
  color: var(--gris-oscuro);
}

@media (min-width: 768px) {
  .contenedor-presupuesto p {
    text-align: left;
  }
}

.contenedor-presupuesto span {
  font-weight: 900;
  color: var(--azul);
}
</style>
