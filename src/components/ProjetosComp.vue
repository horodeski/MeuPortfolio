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
      ImagemProjeto="./src/assets/img/betfreg.png"
      LinkProjeto="https://betfreg.vercel.app/"
      Icone="html5"
      IconeDois="css3"
    />
    <CardProjeto
      NomeProjeto="MAM"
      DescricaoProjeto="Puxando api do TMDB com axios em VueJS"
      ImagemProjeto="./src/assets/img/markantonymovies.png"
      LinkProjeto="https://markantonymovies.surge.sh/"
      Icone="vuejs"
      IconeDois="css3"
    />
    <CardProjeto
      NomeProjeto="Livraria do DUDU"
      DescricaoProjeto="Puxando dados do BackEnd em javascript puro com axios"
      ImagemProjeto="./src/assets/img/livrariadodudu.png"
      LinkProjeto="https://livrariadodudu2.surge.sh/"
      Icone="vuejs"
      IconeDois="heroku"
    />
    <CardProjeto
      NomeProjeto="Calculadora de gorjetas"
      DescricaoProjeto="Calculadora de gorjetas em vue"
      ImagemProjeto="./src/assets/img/calculadora.png"
      LinkProjeto="https://calculadora-gorjetas-nine.vercel.app/"
      Icone="vuejs"
      IconeDois="javascript"
    />
  </div>
</template>
