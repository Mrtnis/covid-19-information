<template>
  <div>
    <Navbar />
    <div class="container">
      <Home />
    </div>
    <Data />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Home from './views/Home.vue';
import Data from './components/Data.vue';

export default {
  components: {
    Navbar,
    Home,
    Data,
  },
};
</script>

<style>
body {
  font-family: 'Roboto', sans-serif;
}
</style>

<style scoped>
.container {
  margin-top: 100px;
  margin-bottom: 40px;
}
</style>
