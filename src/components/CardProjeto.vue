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
    <div class="container">
      <div class="header">
        <div>
          <h3>{{ NomeProjeto }}</h3>
        </div>
        <div>
          <a class="links" target="_blank" :href="LinkGithub">
            <i class="bx bxl-github"></i>
          </a>
          <a class="links" target="_blank" :href="LinkProjeto">
            <i class="bx bx-slideshow"></i>
          </a>
        </div>
      </div>
      <p>{{ DescricaoProjeto }}</p>
    </div>
    <div class="langs">
      <i class="bx bxs-circle"></i>
      <span>Vue</span>
    </div>
  </div>
</template>
<style scoped>
.card {
  width: 48%;
  background-color: #111111;
  padding: 20px;
  border-radius: 5px;
  height: 28vh;
  display: flex;
  margin: 0 10px 25px 10px;
  flex-direction: column;
  justify-content: space-between;
}
.card .langs {
  display: flex;
  gap: 5px;
  align-items: center;
}
.card .langs i {
  color: #29a1d2;
}
.card .header {
  display: flex;
  width: 100%;
  align-items: center;
  justify-content: space-between;
}
.card .header i {
  color: white;
  font-size: 2.5em;
}
.card .header .links i:hover {
  color: #29a1d2;
  cursor: pointer;
  transition: all 0.5s;
}
.card .header h3 {
  text-align: center;
  font-size: 1.5em;
  color: #29a1d2;
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
  border-radius: 5px;

  color: white;
  height: 7vh;
  width: 116px;
}

.mais button:hover {
  border: 4px solid #29a1d2;
  color: #29a1d2;
  transition: 0.5s all;
  cursor: pointer;
}
</style>
