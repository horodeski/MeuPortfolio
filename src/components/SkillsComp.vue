<script setup>
import HH2 from "./template/HH2.vue";

const skills = [
  {
    name: "cool",
    title: "Trabalho em equipe",
    description:
      "capacidade de colaborar com os outros, ser flexível e adaptar-se a diferentes personalidades e estilos de trabalho.",
  },
  {
    name: "shocked",
    title: "Trabalho em equipe",
    description:
      "capacidade de colaborar com os outros, ser flexível e adaptar-se a diferentes personalidades e estilos de trabalho.",
  },
  {
    name: "wink-tongue",
    title: "Criatividade",
    description:
      " a habilidade de pensar fora da caixa para encontrar soluções inovadoras para problema.",
  },
];
</script>
<template>
  <section>
    <h2>Skills</h2>
    <div class="soft-skills">
      <h-h2 tag="h3" text="Soft skills" />
      <div class="cards">
        <div class="card-skills" v-for="(skill, i) in skills" :key="i">
          <box-icon size="5em" color="#fff" :name="skill.name"></box-icon>
          <div>
            <h4>{{ skill.title }}</h4>
            <p>
              {{ skill.description }}
            </p>
          </div>
        </div>
      </div>
    </div>

    <div class="hard-skills">
      <h-h2 tag="h3" text="Hard skills" />
      <div class="logos">
        <div id="efeito" class="card-hard-skills">
          <i class="bx bxl-html5" id="logo-skills"></i>
          <h3>HTML5</h3>
        </div>
        <div id="efeito" class="card-hard-skills">
          <i class="bx bxl-css3" id="logo-skills"></i>

          <h3>CSS3</h3>
        </div>
        <div id="efeito" class="card-hard-skills">
          <i class="bx bxl-javascript" id="logo-skills"></i>
          <h3>JAVASCRIPT</h3>
        </div>
        <div id="efeito" class="card-hard-skills">
          <i class="bx bxl-sass" id="logo-skills"></i>
          <h3>SASS</h3>
        </div>
        <div id="efeito" class="card-hard-skills">
          <i class="bx bxl-vuejs" id="logo-skills"></i>
          <h3>VUEJS</h3>
        </div>
        <div id="efeito" class="card-hard-skills">
          <i class="bx bxl-git" id="logo-skills"></i>
          <h3>GIT</h3>
        </div>
        <div id="efeito" class="card-hard-skills">
          <i class="bx bxl-github" id="logo-skills"></i>
          <h3>GITHUB</h3>
        </div>
        <div id="efeito" class="card-hard-skills">
          <i class="bx bxl-django" id="logo-skills"></i>
          <h3>DJANGO</h3>
        </div>
        <div id="efeito" class="card-hard-skills">
          <i class="bx bxl-react" id="logo-skills"></i>
          <h3>REACT NATIVE</h3>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
section {
  display: flex;
  flex-direction: column;
  align-items: center;
}
section .logos {
  display: flex;
  flex-wrap: wrap;
}
section .soft-skills .cards {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: center;
}

section .soft-skills .card-skills {
  width: 31%;
  display: flex;
  margin: 10px;
  border-radius: 17px;
  padding: 13px;
  background-color: #111;
  align-items: center;
  justify-content: flex-start;
  flex-direction: column;
  transition: transform 1s;
  transform: scale(90%);
}

section .soft-skills .card-skills:hover {
  border: 2px solid #29a1d2;
  transform: scale(100%);
  cursor: pointer;
}

section .soft-skills .card-skills div {
  display: flex;
  flex-direction: column;
  align-items: center;
}

section .soft-skills .card-skills div p {
  text-align: center;
}

section .soft-skills .card-skills div h4 {
  color: #29a1d2;
  font-size: 1.4em;
}

section .hard-skills .logos .card-hard-skills {
  display: flex;
  flex-direction: column;
  color: #ffffff;
  border-radius: 17px;
  margin: 6px;
  padding: 10px;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
}
section .hard-skills .logos .card-hard-skills .logo-skills {
  width: 6rem;
  height: 5rem;
}
section .hard-skills .logos .card-hard-skills:hover {
  background-color: #111;
  color: #29a1d2;
  cursor: pointer;
}

#efeito {
  width: 200px;
  border: 18px solid #0009;
  transition: 0.6s;
}
#efeito:hover {
  border: 2px solid #29a1d2;
}

section .hard-skills .logos .card-hard-skills #logo-skills {
  font-size: 7em;
}

section .hard-skills {
  width: 100%;
}
</style>
