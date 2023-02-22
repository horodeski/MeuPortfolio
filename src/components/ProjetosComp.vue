<script>
import CardProjeto from "../components/CardProjeto.vue";
export default {
  components: {
    CardProjeto,
  },
};
</script>
<template>
  <h2>Projetos</h2>
  <div class="todos-projetos">
    <CardProjeto
      NomeProjeto="BETFREG"
      DescricaoProjeto="Landing page responsiva"
      ImagemProjeto="/src/assets/img/betfreg.png"
      Icone="html5"
      IconeDois="css3"
    />
    <CardProjeto
      NomeProjeto="MAM"
      DescricaoProjeto="Puxando api do TMDB com axios em VueJS"
      ImagemProjeto="/src/assets/img/markantonymovies.png"
      Icone="vuejs"
      IconeDois="css3"
    />
    <CardProjeto
      NomeProjeto="Livraria do DUDU"
      DescricaoProjeto="Puxando dados do BackEnd em javascript puro com axios"
      ImagemProjeto="/src/assets/img/livrariadodudu.png"
      Icone="vuejs"
      IconeDois="heroku"
    />
    <CardProjeto
      NomeProjeto="Calculadora de gorjetas"
      DescricaoProjeto="Calculadora de gorjetas em vue"
      ImagemProjeto="/src/assets/img/calculadora.png"
      Icone="vuejs"
      IconeDois="javascript"
    />
  </div>
</template>
