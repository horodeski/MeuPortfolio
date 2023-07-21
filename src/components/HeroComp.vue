<script>
export default {};
</script>
<template>
  <section class="hero-comp">
    <div class="apresentacao">
      <h2>Olá, tudo bem?</h2>
      <h1>
        Me chamo
        <span> Geovana Horodeski </span>
        :)
      </h1>
      <p>
        Este é o portfolio de uma profissional apaixonada por tecnologia e que
        pretende trabalhar com desenvolvimento.
      </p>
      <box-icon
        name="down-arrow-square"
        size="lg"
        class="floating"
        type="solid"
        color="#29A1D2"
      ></box-icon>
    </div>
  </section>
</template>
<style scoped>
.hero-comp {
  background: url(/src/assets/img/computador.gif) no-repeat;
  background-size: cover;
  background-attachment: fixed;
  background-position: center;
  height: 100vh;
  margin-bottom: 30px;
}

.apresentacao {
  display: flex;
  flex-direction: column;
  height: 100vh;
  width: 100%;
  background-color: #000000bd;
  align-items: center;
  justify-content: center;
}

.apresentacao span {
  color: #29A1D2;
}
.apresentacao h1 {
  font-size: 3em;
  margin-top: -22px;
}

.apresentacao p {
  width: 46%;
  margin-top: -12px;
  text-align: center;
}
.floating {
  animation-name: floating;
  animation-duration: 3s;
  animation-iteration-count: infinite;
  animation-timing-function: ease-in-out;
  margin-left: 30px;
  margin-top: 5px;
}

@keyframes floating {
  0% {
    transform: translate(0, 0px);
  }

  50% {
    transform: translate(0, 15px);
  }

  100% {
    transform: translate(0, -0px);
  }
}

</style>
