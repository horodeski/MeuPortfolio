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
<style scoped>
.card {
  width: 48%;
  background-color: #111111;
  padding: 8px 20px;
  border-radius: 17px;
  display: flex;
  margin: 0 10px 25px 10px;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
}
.card .infos {
  display: flex;
  width: 100%;
  align-items: center;
  justify-content: space-between;
}
.card .infos i {
  color: white;
  font-size: 4em;
}
.card .infos .links i:hover {
  color: #29A1D2;
  cursor: pointer;
  transition: all 0.5s;
}
.card .infos h3{
  text-align: center;
  font-size: 1.5em;
  color: #29A1D2;
}
.mais {
  display: flex;
  align-items: center;
  width: 100%;
  justify-content: space-around;
}

.mais button {
  background-color: transparent;
  border: 4px solid white;
  /* padding: 14px 20px; */
  border-radius: 17px;

  color: white;
  height: 7vh;
  width: 116px;
}

.mais button:hover {
  border: 4px solid #29A1D2;
  color: #29A1D2;
  transition: 0.5s all;
  cursor: pointer;
}

.card img {
  border-radius: 17px;

  width: 100%;
}

</style>