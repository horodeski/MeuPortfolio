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
</template>
