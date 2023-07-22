<script setup></script>
<template>
  <section id="sobre-mim">
    <h2>Sobre mim</h2>
    <div class="eu">
      <img src="/src/assets/img/eu.jpg" alt="eu" />
      <div>
        <h2>Geovana Horodeski</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sunt culpa,
          earum dolorum odit laborum iusto, vel pariatur consectetur nemo nisi
          blanditiis cupiditate? Dolores facilis delectus voluptas architecto a,
          consequuntur corrupti.
        </p>
      </div>
    </div>
  </section>
</template>
<style scoped>
.eu img {
  width: 30%;
  border-radius: 50%;
  margin-right: 45px;
}

section {
  display: flex;
  flex-direction: column;
  align-items: center;
}

section {
  display: flex;
}

section .eu {
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-evenly;
}

section .eu .infos {
  display: flex;
  justify-content: space-between;
  flex-direction: row;
}

section .eu .infos h3 {
  color: #29a1d2;
  font-size: 1.3em;
}
section .eu .infos h4 {
  font-size: 1.2em;
  font-weight: 100;
}
section .eu-interesses {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>
