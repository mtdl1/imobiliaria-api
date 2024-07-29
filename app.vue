<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout> 
  </div>
</template>

<script setup lang="ts">
useSeoMeta({
  title: 'Anima Signature',
  ogTitle: 'Empreendimento Alto Luxo em Belo Horizonte',
  ogDescription: 'Conheça o Anima Signature, um empreendimento de alto luxo em Belo Horizonte. Apartamentos de 4 quartos com 4 suítes e 4 vagas de garagem.',
  ogImage: '/predio-anima.jpg',
  ogUrl: 'https://anima-signature.com.br',
  twitterTitle: 'Empreendimento Alto Luxo em Belo Horizonte',
  twitterDescription: 'Conheça o Anima Signature, um empreendimento de alto luxo em Belo Horizonte. Apartamentos de 4 quartos com 4 suítes e 4 vagas de garagem.',
  twitterImage: '/predio-anima.jpg',
})
</script>
