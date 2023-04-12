<script>
export default {
  props: {
    NomeProjeto: String,
    DescricaoProjeto: String,
    ImagemProjeto: String,
    Icone: String,
    IconeDois: String,
    LinkProjeto: String,
  },
};
</script>
<template>
  <div class="card">
    <img :src="ImagemProjeto" alt="" />
    <div class="infos">
      <h2>{{ NomeProjeto }}</h2>
      <p>{{ DescricaoProjeto }}</p>
    </div>
    <div class="mais">
      <a :href="LinkProjeto">
        <button>detalhes</button>
      </a>
      <div>
        <box-icon
          size="lg"
          class="logo-skills"
          :name="Icone"
          type="logo"
          color="#ffffff"
        ></box-icon>
        <box-icon
          size="lg"
          class="logo-skills"
          :name="IconeDois"
          type="logo"
          color="#ffffff"
        ></box-icon>
      </div>
    </div>
  </div>
</template>
