<script setup>
const sections = document.querySelectorAll("section");
const Link = document.querySelectorAll(".container a");
document.documentElement.style.scrollBehavior = "smooth";

window.onscroll = () => {
  let current = null;

  sections.forEach((section) => {
    const sectionTop = section.offsetTop;
    const offset = 60;

    if (window.scrollY + offset >= sectionTop) {
      current = section.getAttribute("id");
    }
  });

  Link.forEach((a) => {
    a.classList.remove("active");
    if (current && a.classList.contains(current)) {
      a.classList.add("active");
    }
  });
};
</script>
<template>
  <section class="hero-comp">
    <div class="apresentacao">
      <div class="container">
        <h2>Olá, tudo bem?</h2>
        <h1>
          Me chamo
          <span> Geovana Horodeski </span>
          :)
        </h1>
        <p id="effect">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat,
          beatae natus facere dolorem excepturi laboriosam voluptas temporibus,
          velit, ipsum cum quos animi alias reprehenderit repudiandae? Sunt
          tempora vitae dolorem harum.
        </p>
        <a href="#sobre-mim">
          <box-icon
            name="mouse"
            size="lg"
            class="floating"
            color="#29A1D2"
          ></box-icon>
        </a>
      </div>
    </div>
  </section>
</template>
<style scoped>
span {
  border-right: 0.05em solid;
  animation: caret 1s steps(1) infinite;
}

@keyframes caret {
  50% {
    border-color: transparent;
  }
}
.hero-comp {
  background: url(/src/assets/img/computador.gif) no-repeat;
  background-size: cover;
  background-attachment: fixed;
  background-position: center;
  height: 100vh;
  margin-bottom: 30px;
}
.apresentacao .container {
  display: flex;
  flex-direction: column;
  /* height: 40vh; */
  align-items: center;
  justify-content: center;
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
  color: #29a1d2;
}
.apresentacao h1 {
  font-size: 3em;
}

.apresentacao p {
  width: 46%;
  text-align: center;
}
.apresentacao h2 {
  margin: 0;
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
