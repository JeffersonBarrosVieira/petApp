<template>
  <nav id="nav">
    <router-link to="/" id="logo-url">
      <img :src="logo" :alt="alt" id="logo" />
    </router-link>
    <router-link to="/">Home</router-link>
    <router-link to="/about">Sobre</router-link>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  props: ["logo", "alt"]
};
</script>

<style scoped>
#nav {
  background-color: #7f00b2;
  border-bottom: 4px solid #ab3ed8;
  padding: 15px 50px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

#nav #logo-url {
  margin: auto;
  margin-left: 0;
  border: 2px solid var(--branco);
  border-radius: 10px;
}

#logo {
  width: 40px;
  height: 40px;
}

#nav a {
  color: var(--branco);
  font-weight: bold;
  text-decoration: none;
  margin: 12px;
  transition: .5s;
}

#nav a:hover{
  color: var(--branco);
}
</style>
