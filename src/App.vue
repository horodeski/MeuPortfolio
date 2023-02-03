<script setup>
import HeaderComp from "./components/HeaderComp.vue";
import ContatoComp from "./components/ContatoComp.vue";
import SobreMimComp from "./components/SobreMimComp.vue";
</script>

<template>
  <aside class="contatos">
    <ContatoComp />
  </aside>
  <aside class="home">
    <img src="/src/assets/img/logo.png" alt="">
  </aside>
  <header>
    <HeaderComp />
  </header>
  <main>
    <section class="sobre-mim">
      <SobreMimComp />
    </section>
  </main>
</template>

<style></style>
