<template>
  <div>
    <Header />
    <main>
      <Hero />
      <Services />
      <Work />
    </main>
    <Footer />
  </div>
</template>

<script setup>
useHead({
  title: 'Front-end developer & interaction designer - Bram Doppen',
  meta: [
    { name: 'description', content: 'Als ervaren frontend developer ben ik gepassioneerd over het creëren van "vette shit" en het vinden van de balans tussen complexiteit en gebruiksvriendelijkheid. Ontdek hoe ik nieuwe technieken omarm om kwaliteit te leveren.' }
  ],
  bodyAttrs: {
    class: 'test'
  },
  script: [{ innerHTML: 'console.log(\'Hello world\')' }]
})
</script>
