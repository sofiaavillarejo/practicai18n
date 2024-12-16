<template>
  <div>
    <button class="flag-button">
      <img style="width: 50px;" alt="Change language" />
    </button>
    <div class="d-flex justify-content-center mt-3">
      <form class="w-50 p-4 rounded shadow-lg bg-light">
        <h2 class="text-center mb-4">Hola, bienvenido!</h2>

        <div class="mb-3">
          <label class="form-label fw-bold">Nombre</label>
          <input class="form-control" type="text" placeholder="Escribe tu nombre">
        </div>

        <div class="mb-3">
          <label class="form-label fw-bold">Apellido</label>
          <input class="form-control" type="text" placeholder="Escribe tu apellido"/>
        </div>

        <div class="text-center">
          <button type="submit" class="btn btn-success btn-lg px-5">Enviar</button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PruebaComponent',
  methods: {
    changeLanguage() {
      this.$i18n.locale = this.$i18n.locale === 'en' ? 'es' : 'en';
    }
  }
};
</script>
<style>
  .flag-button {
    font-size: 1.5rem;
    background: none;
    border: none;
    cursor: pointer;
  }
  
</style>