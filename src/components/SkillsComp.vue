<script setup>
import HH2 from './template/HH2.vue';

const skills = [
  {
    name: "cool",
    title: "Trabalho em equipe",
    description: "capacidade de colaborar com os outros, ser flexível e adaptar-se a diferentes personalidades e estilos de trabalho."
  },
  {
    name: "shocked",
    title: "Trabalho em equipe",
    description: "capacidade de colaborar com os outros, ser flexível e adaptar-se a diferentes personalidades e estilos de trabalho."
  },
  {
    name: "wink-tongue",
    title: "Criatividade",
    description: " a habilidade de pensar fora da caixa para encontrar soluções inovadoras para problema."
  }
]
</script>
<template>
  <h2>Skills</h2>
  <div class="soft-skills">
    <h-h2 text="Soft skills" />
    <div class="cards" >
      <div class="card-skills" v-for="(skill, i) in skills" :key="i">
        <box-icon size="5em" color="#fff" :name="skill.name"></box-icon>
        <div>
          <h3>{{skill.title}}</h3>
          <p>
            {{skill.description}}
          </p>
        </div>
      </div>
      <!-- <div class="card-skills">
        <box-icon size="5em" name="shocked" color="#ffffff"></box-icon>
        <div>
          <h3>Resolução de problemas</h3>
          <p>a habilidade de identificar e resolver problemas técnicos.</p>
        </div>
      </div>
      <div class="card-skills">
        <box-icon size="5em" name="wink-tongue" color="#ffffff"></box-icon>
        <div>
          <h3>Criatividade</h3>
          <p>
            a habilidade de pensar fora da caixa para encontrar soluções
            inovadoras para problema.
          </p>
        </div>
      </div> -->
    </div>
  </div>

  <div class="hard-skills">
    <h-h2 text="Hard skills" />
    <div class="logos">
      <div class="card-hard-skills">
        <!--TEM QUE ARRUMAR ESSA BOMBA AQUI-->
        <box-icon
          size="lg"
          class="logo-skills"
          name="html5"
          type="logo"
          color="#ffffff"
        ></box-icon>
        <h3>HTML5</h3>
      </div>
      <div class="card-hard-skills">
        <box-icon
          size="lg"
          class="logo-skills"
          name="css3"
          type="logo"
          color="#ffffff"
        ></box-icon>
        <h3>CSS3</h3>
      </div>
      <div class="card-hard-skills">
        <box-icon
          size="lg"
          class="logo-skills"
          name="javascript"
          type="logo"
          color="#ffffff"
        ></box-icon>
        <h3>JAVASCRIPT</h3>
      </div>
      <div class="card-hard-skills">
        <box-icon
          size="lg"
          class="logo-skills"
          name="sass"
          type="logo"
          color="#ffffff"
        ></box-icon>
        <h3>SASS</h3>
      </div>
      <div class="card-hard-skills">
        <box-icon
          size="lg"
          class="logo-skills"
          name="vuejs"
          type="logo"
          color="#ffffff"
        ></box-icon>
        <h3>VUEJS</h3>
      </div>
      <div class="card-hard-skills">
        <box-icon
        size="lg"
        class="logo-skills"
        name="git"
        type="logo"
          color="#ffffff"
          ></box-icon>
          <h3>GIT</h3>
        </div>
      <div class="card-hard-skills">
        <box-icon
          size="lg"
          class="logo-skills"
          name="github"
          type="logo"
          color="#ffffff"
          ></box-icon>
          <h3>GITHUB</h3>
      </div>
      <div class="card-hard-skills">
        <box-icon
          size="lg"
          class="logo-skills"
          name="django"
          type="logo"
          color="#ffffff"
        ></box-icon>
        <h3>DJANGO</h3>
      </div>
      <div class="card-hard-skills">
        <box-icon
          size="lg"
          class="logo-skills"
          name="react"
          type="logo"
          color="#ffffff"
          ></box-icon>
          <h3>REACT NATIVE</h3>
      </div>
    </div>
  </div>
</template>
