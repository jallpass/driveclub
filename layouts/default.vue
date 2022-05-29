<template>
  <div class="container">
    <AppHeader/>
    <nuxt/>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from "../components/AppHeader";
import AppFooter from "../components/AppFooter";

export default {
  components: {
    AppHeader,
    AppFooter
  }
};
</script>


<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 1rem;
  line-height: 1.6;
  background: #f4f4f4;
}

a {
  color: #ffffff;
  text-decoration: none;
}

ul {
  list-style: none;
}

label {
  color: #ffffff;
}

.container {
  max-width: 100%;
  overflow: hidden;
  padding: 0;
  background: #171B1E;
}
</style>
