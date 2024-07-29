<template>
  <div class="totalLocMap">
    <div class="conteudo-texto">
      <h2>Lorem ipsum dolor sit amet consectetur</h2>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolorum explicabo consequatur similique quam, suscipit vitae velit ut eaque eligendi excepturi. Exercitationem modi porro libero? Repellendus nostrum ipsum ratione perferendis odit?</p>
      <p><strong>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa velit dicta consectetur expedita eligendi sequi deserunt voluptas obcaecati illo, dolor veritatis autem animi quam aspernatur, nostrum vitae in similique alias?</strong></p>
      <!-- Botao ir com Waze -->
      <div class="waze">
        <a href="https://waze.com/ul?ll=-23.5505199,-46.6333094&navigate=yes" target="_blank">
          <img src="/icons/waze-icon.svg"/>
          <p>Ir com Waze</p>
        </a>
      </div>
    </div>
    <div class="mapa">
      <!-- Não tenho API ainda para usar o GmapMap -->
      <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d15002.884084380888!2d-43.9371775!3d-19.9361577!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xa699dbbadbffff%3A0xd895dc03c63496dc!2s%C3%82nima%20Signature!5e0!3m2!1spt-BR!2sbr!4v1722287598998!5m2!1spt-BR!2sbr" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    </div>
    <div class="localizacoes">
      <div class="localizacao">
        <img src="/icons/map-pin.svg"/>
        <p><span>Prédio Ipsum</span> 18.6km</p>
      </div>
      <div class="localizacao">
        <img src="/icons/map-pin.svg"/>
        <p><span>Prédio Ipsum</span> 32.6km</p>
      </div>
      <div class="localizacao">
        <img src="/icons/map-pin.svg"/>
        <p><span>Prédio Ipsum</span> 45km</p>
      </div>
      <div class="localizacao">
        <img src="/icons/map-pin.svg"/>
        <p><span>Prédio Ipsum</span> 56.2km</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.totalLocMap {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  max-width: 70%;
  margin: 5% auto;
  padding: 5% 0;
  border-radius: 20px;
  background-color: #FFF;
}

.conteudo-texto {
  width: 45%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 20px;
}

.titulo {
  width: 100%;
}

h2 {
  font-size: 2rem;
  margin-bottom: 4%;
  border-left: 5px solid cornflowerblue;
  padding-left: 15px;
}

.conteudo-texto p {
  font-size: 1.2rem;
  margin-bottom: 4%;
}

strong {
  font-weight: 700;
}

.waze {
  width: 30%;
  padding: 1% 4%;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 20px;
  background-color: #31cdfe;
}

.waze img{
  max-width: 25px;
}

.waze p{
  /* font-size: 1rem; */
  font-weight: 700;
  color: white;
}

a {
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  color: black;
}

img {
  margin-right: 10px;
}

.mapa {
  width: 45%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 20px;
}

.mapa iframe {
  border-radius: 20px;
}

.localizacoes {
  width: 90%;
  margin-top: 5%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.localizacao {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 10px;
}

.localizacao img {
  margin-right: 10px;
}

.localizacao p {
  font-size: 1.2rem;
}

.localizacao span {
  text-decoration: underline;
  color: darkslategray;
}

/* responsivo */
@media (max-width: 768px) {
  .totalLocMap {
    max-width: 90%;
    margin: 15% auto;
  }

  h2{
    font-size: 1.5rem;
  }

  .conteudo-texto {
    width: 100%;
  }

  .conteudo-texto p {
    font-size: 1rem;
  }

  .waze {
    width: 100%;
  }

  .mapa {
    width: 90%;
  }

  .localizacoes {
    flex-direction: column;
  }

  .localizacao {
    margin: 10px 0;
  }
}

</style>