<template>
  <div>
    <div class="beneficios">
      <div class="beneficio">
        <img src="/icons/planta-icon.svg" alt="">
        <h3>Lotes á partir de 92m²</h3>
        <p>Residenciais e Comerciais</p>
      </div>
      <div class="beneficio">
        <img src="/icons/papelada-icon.svg" alt="">
        <h3>Documentação Grátis</h3>
      </div>
      <div class="beneficio">
        <img src="/icons/parque-icon.svg" alt="">
        <h3>Área de Lazer Completa</h3>
      </div>
      <div class="beneficio">
        <img src="/icons/bola-icon.svg" alt="">
        <h3>Quadra Poliesportiva</h3>
      </div>
    </div>
  </div>
</template>

<style scoped>
.beneficios {
  max-width: 70%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 5vh 0;
  margin: 0 auto;
  gap: 2vw;
}

.beneficio {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  width: 24%;
  background-color: #FAFAFA;
  height: 15vh;
  text-align: center;
  padding: 20px;
  border-radius: 10px;
}

.beneficio img {
  max-width: 50%;
}

.beneficio h3 {
  font-size: 1.2rem;
  width: 100%;
  font-weight: 600;
}

.beneficio p {
  font-size: 1rem;
  font-weight: 300;
  line-height: 1.5;
}

/* responsivo */
@media (max-width: 768px) {
  .beneficios{
    max-width: 90%;
    flex-wrap: wrap;
  }

  .beneficio {
    width: 48%;
    height: 20vh;
  }
}

</style>