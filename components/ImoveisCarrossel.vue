<template>
  <div class="main-imoveis">
    <h2>Últimos lançamentos excluisivos de alto luxo em BH</h2>
    <!-- <div class="imoveis">
      <div class="imovel" v-for="imovel in data.imoveis" :key="imovel.id">
        <img src="/predio-anima.jpg" alt="">
        <h3>{{ imovel.Nome }}</h3>
        <p>R$ {{ imovel.Valor }}</p>
        <p>Status: {{ imovel.status }}</p>
      </div>
    </div> -->

    <div class="carrosel-imoveis">
      <Splide :options="options">
        <SplideSlide v-for="imovel in data.imoveis.imovel" :key="imovel.id">
          <div class="imovel">
            <img src="/predio-anima.jpg" alt="">
            <h3>{{ imovel.Nome }}</h3>

            <p v-if="imovel.status === 1">Em construção</p>
            <p v-if="imovel.status === 2">Pronto para morar</p>
            <p v-if="imovel.status === 3">100% Vendido</p>

            <p> a partir de <span>R$ {{ imovel.Valor }}</span></p>
          </div>
        </SplideSlide>
      </Splide>
    </div>

  </div>
</template>

<script setup lang="ts">
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/vue-splide/css/sea-green';

const { data: data } = await useFetch('https://298dc7b0d9ef4714a086a3c09c305965.api.mockbin.io/');

const options = {
  type: 'loop',
  perPage: 3,
  perMove: 1,
  gap: '1rem',
  pagination: false,
  breakpoints: {
    768: {
      perPage: 1,
      gap: '0',
    },
  },
};


</script>

<style scoped>

.main-imoveis {
  background-color: #FAFAFA;
  padding: 5vh 0;
}

h2{
  text-align: center;
  margin: 5vh 0;
  font-size: 3rem;
  font-weight: 600;
  color: #333;
}

.carrosel-imoveis {
  width: 70%;
  margin: 0 auto;
}

/* .imoveis {
  max-width: 70%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 5vh 0;
  margin: 0 auto;
  gap: 2vw;
} */

.imovel {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  background-color: #eeeeee;
  text-align: center;
  border-radius: 10px;
  padding-bottom: 10px;
}

.imovel img {
  border-radius: 10px 10px 0 0;
}

.imovel h3 {
  font-size: 1.2rem;
  width: 100%;
  font-weight: 600;
  padding-top: 10px;
}

.imovel p {
  font-size: 1rem;
  width: 100%;
  padding-top: 10px;
}

/* responsivo */
@media (max-width: 768px) {
  h2{
    font-size: 1.5rem;
    padding: 0 10%;
  }
}

</style>
