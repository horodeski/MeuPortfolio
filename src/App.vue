<script>
import HeroComp from "./components/HeroComp.vue";
import ContatoComp from "./components/ContatoComp.vue";
import SobreMimComp from "./components/SobreMimComp.vue";
import SkillsComp from "./components/SkillsComp.vue";
import ProjetosComp from "./components/ProjetosComp.vue";
export default {
  components: {
    HeroComp,
    ContatoComp,
    SobreMimComp,
    SkillsComp,
    ProjetosComp,
  },
};
</script>

<template>
  <ContatoComp />
  <HeroComp />
  <main>
    <SobreMimComp />
    <SkillsComp />
    <ProjetosComp />
  </main>
</template>

<style></style>
