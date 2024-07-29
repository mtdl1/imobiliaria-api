<template>
  <footer>
    <img class="logo-anima" src="/icons/logo-imobiliaria.svg" alt="Logo" />
    <div class="sociais">
      <a href="https://www.linkedin.com" target="_blank">
        <img src="/icons/linkedin-logo.svg" alt="Linkedin" />
      </a>
      <a href="https://www.instagram.com" target="_blank">
        <img src="/icons/instagram-logo.svg" alt="Instagram" />
      </a>
      <a href="https://www.youtube.com" target="_blank">
        <img src="/icons/youtube-logo.svg" alt="Youtube" />
      </a>
    </div>
    <p class="direitos">&copy; Anima Signature - 2024 - Todos os direitos reservados</p>
  </footer>
</template>

<style scoped>
footer {
  color: #FAFAFA;
  text-align: center;
  padding: 2% 0;
  border-top: 1px solid #555;
}

.logo-anima {
  max-width: 6%;
}

.sociais {
  display: flex;
  justify-content: center;
  margin-top: 2%;
  gap: 2%;
}

.sociais a{
  background-color: #FAFAFA;
  padding: 15px;
  border-radius: 50%;
  cursor: pointer;
}

.direitos {
  margin-top: 2%;
}

/* responsivo */
@media (max-width: 768px) {
  footer {
    padding: 20% 0;
  }

  .logo-anima {
    max-width: 25%;
  }

  .sociais {
    margin-top: 8%;
    gap: 8%;
  }

  .sociais a{
    padding: 10px;
  }

  .direitos {
    margin-top: 8%;
    font-size: 0.7rem;
  }

}
</style>
