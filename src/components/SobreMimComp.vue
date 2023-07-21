<script setup>
import HH2 from "./template/HH2.vue";
</script>
<template>
  <section>
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
  </section>
</template>
<style scoped>

.eu img {
  width: 20%;
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
  margin: 30px 0;
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
  color: #29A1D2;
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