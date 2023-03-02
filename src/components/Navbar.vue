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

