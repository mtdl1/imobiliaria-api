<template>
  <div class="banner-main">
    <div class="content">
      <p><span>Breve Lançamento</span></p>
      <h1>Chegou a sua vez de viver bem</h1>
      <p><strong>Lotes de 92 à 198m², próximos ao shopping</strong></p>
      <p class="text">ÂNIMA significa alma, algo que é único e complexo ao mesmo tempo. Cada alma é como uma impressão digital, carregando nossas histórias, sonhos e desejos.</p>
    </div>
  </div>
</template>

<style scoped>
.banner-main {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  background:linear-gradient(0deg, rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.5)), url(/banner-anima.png);
}

.content {
  text-align: center;
  color: white;
  font-size: 1.5rem;
  padding: 11vh 0;
  width: 70%;
  text-align: left;
}

.content p {
  margin: 1vh 0;
}

.content p span {
  font-size: 0.8rem;
}

.content h1 {
  font-size: 2.5rem;
  margin: 2vh 0;
  padding-right: 30%;
  font-weight: 700;
}

.content strong {
  font-size: 1.5rem;
  margin: 2vh 0;
  font-weight: 600;
}

.content p.text {
  margin-top: 2vh;
  font-size: 1rem;
  font-weight: 300;
  line-height: 1.5;
}

</style>