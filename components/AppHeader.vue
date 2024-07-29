<template>
  <div>
    <header>
      <div class="logo">
        <img src="/icons/logo-imobiliaria.svg" alt="Logo" />
      </div>
    </header>
  </div>
</template>

<style scoped>
header{
  padding: 2% 0;
  width: 70%;
  margin: 0 auto;
  background: transparent;
}

.logo{
  position: absolute;
}

.logo img{
  max-width: 6%;
  position: relative;
  bottom: -20px;
}

/* responsivo */
@media (max-width: 768px) {
  header{
    width: 100%;
  }

  .logo{
    width: 100%;
    text-align: center;
    position: unset;
  }

  .logo img{
    max-width: 25%;
  }
}
</style>

