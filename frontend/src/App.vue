<template>
  <div id="app">
    
      <Nav />
    
    <router-view :key="$route.fullPath"></router-view>
  </div>
</template>

<script>
import Nav from "./components/Nav.vue";

export default {
  name: "App",
  components: { Nav }
};
</script>

<style lang="css">
a {
  text-decoration: none;
  color: rgb(196, 112, 3) !important;
  position: relative !important;
}

a::before {
  content: "";
  position: absolute;
  width: 40%;
  height: 2px;
  background-color: burlywood;
  bottom: 25px;
  left: 17px;
}

a:hover {
  color: rgb(212, 145, 82) !important;
}

h1 {
  font-family: Staatliches;
  font-size: 120px;
}

#category {
  font-family: Staatliches;
  font-weight: 500;
}

#title {
  letter-spacing: 0.4px;
  font-size: 22px;
  font-size: 1.375rem;
  line-height: 1.13636;
}

#banner {
  margin: 20px;
  height: 800px;
}

#editor {
  font-size: 16px;
  font-size: 1rem;
  line-height: 1.75;
}

.uk-navbar-container {
  background: rgba(255, 255, 255, 0.897) !important;
  font-family: Staatliches;
}

img:hover {
  opacity: 1;
  transition: opacity 0.25s cubic-bezier(0.39, 0.575, 0.565, 1);
}
</style>
