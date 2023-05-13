<script>
export default {
  props: {
    NomeProjeto: String,
    DescricaoProjeto: String,
    ImagemProjeto: String,
    Icone: String,
    IconeDois: String,
    LinkProjeto: String,
    LinkGithub: String,
  },
};
</script>
<template>
  <div class="card">
    <div class="infos">
      <div>
        <i class="bx bx-box"></i>
      </div>
      <div>
        <h3>{{ NomeProjeto }}</h3>
      </div>
      <div>
        <a class="links" target="_blank" :href="LinkGithub">
          <i class="bx bxl-github"></i>
        </a>
        <a class="links" target="_blank" :href="LinkProjeto">
          <i class="bx bx-layout"></i>
        </a>
      </div>
    </div>
    <p>{{ DescricaoProjeto }}</p>
  </div>
</template>
