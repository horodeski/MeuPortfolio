<script setup>
import HH2 from "./template/HH2.vue";
</script>
<template>
  <h2>Sobre mim</h2>
  <div class="eu">
    <img src="/src/assets/img/eu.jpg" alt="eu" />
    <div>
      <!--! olho nessa duds -->
      <h-h2
        id="teste"
        tag="p"
        text="Sou uma desenvolvedora
        FullStack apaixonada por criar soluções web incríveis e
        intuitivas para os usuários."
      />

      <div class="infos">
        <div>
          <div>
            <h3>NOME:</h3>
            <h4>Geovana Sophia Horodeski</h4>
          </div>
          <div>
            <h3>NASCIMENTO:</h3>
            <h4>3 de julho de 2006</h4>
          </div>
          <div>
            <h3>EMAIL:</h3>
            <h4>geovana.horodeski06@gmail.com</h4>
          </div>
        </div>
        <div>
          <div>
            <h3>BIO:</h3>
            <h4>Gosto de ABBA, filmes e FrontEnd</h4>
          </div>
          <div class="eu-interesses">
            <div>
              <h3>Interesses:</h3>
              <div>
                <box-icon
                  size="lg"
                  color="#ffffff"
                  type="logo"
                  name="css3"
                ></box-icon>
                <box-icon
                  size="lg"
                  name="camera-movie"
                  type="solid"
                  color="#ffffff"
                ></box-icon>
                <box-icon
                  size="lg"
                  type="logo"
                  name="imdb"
                  color="#ffffff"
                ></box-icon>
                <box-icon size="lg" name="music" color="#ffffff"></box-icon>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
