<script>
export default {};
</script>
<template>
  <aside>
    <a class="home" href="src/App.vue">
      <img src="@/assets/img/logo.png" alt="" />
    </a>
    <div>
      <a href="https://github.com/horodeski">
        <box-icon
          size="md"
          name="github"
          type="logo"
          color="#ffffff"
        ></box-icon>
      </a>
      <!--arrumar o linkedin-->
      <a href="https://github.com/horodeski">
        <box-icon
          size="md"
          name="linkedin-square"
          type="logo"
          color="#ffffff"
        ></box-icon>
      </a>
      <hr />
    </div>
  </aside>
</template>
<style scoped>
aside {
  display: flex;
  position: fixed;
  width: 10%;
  height: 100vh;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
}

aside div {
  display: flex;
  flex-direction: column;
  align-items: center;
}

aside hr {
  background-color: white;
  height: 20vh;
  width: 6px;
}

aside img {
  width: 86px;
}

</style>
