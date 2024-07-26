<template>
  <div>
    <header>
      <div class="logo">
        <!-- importar logo svg que ta na pasta public -->
        <img src="/logo-imobiliaria.svg" alt="Logo" />
      </div>
    </header>
  </div>
</template>

<style scoped>
header{
  background: linear-gradient(109.6deg, rgba(0, 0, 0, 0.93) 11.2%, rgb(63, 61, 61) 78.9%);
  padding: 2% 8%;
}

.logo{
  position: absolute;
}

.logo img{
  max-width: 5%;
  position: relative;
  bottom: -20px;
}
</style>

