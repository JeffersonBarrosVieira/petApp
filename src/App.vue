<template>
  <Navbar :logo="logo_src" :alt="app_name" />
  <router-view />
  <Footer />
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Footer,
  },
  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Tudo para o seu Pet"
    }
  }
};
</script>

<style>

/* Variaveis globais */

:root {
  --roxo-1: #7f00b2;
  --roxo-2: #ab32d8;

  --ciano-1: #00cbcc;
  --ciano-2: #00e5e5;
  --ciano-3: #00ffff;

  --branco: #fff;
}

* {
  font-family: Helvetica;
  margin: 0;
  padding: 0;
  box-sizing: 0;
}

.main-container {
  margin: 50px;
  min-height: 300px;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
