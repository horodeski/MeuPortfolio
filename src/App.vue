<script>
import HeaderComp from "./components/HeaderComp.vue";
import ContatoComp from "./components/ContatoComp.vue";
import SobreMimComp from "./components/SobreMimComp.vue";
import FormacaoComp from "./components/FormacaoComp.vue";
import SkillsComp from "./components/SkillsComp.vue";
import ProjetosComp from "./components/ProjetosComp.vue";
export default {
  components: {
    HeaderComp,
    ContatoComp,
    SobreMimComp,
    FormacaoComp,
    SkillsComp,
    ProjetosComp,
  },
};
</script>

<template>
  <aside class="contatos">
    <ContatoComp />
  </aside>
  <aside class="home">
    <a href="#home">
      <img src="@/assets/img/logo.png" alt="" />
    </a>
  </aside>
  <header>
    <HeaderComp />
  </header>
  <main>
    <section class="sobre-mim">
      <SobreMimComp />
    </section>
    <section class="formacao">
      <FormacaoComp />
    </section>
    <section class="skills">
      <SkillsComp />
    </section>
    <section class="projetos">
      <ProjetosComp />
    </section>
  </main>
</template>

<style></style>
