<template>
  <div>
    <Navbar />
    <div class="home-page">
      <Home />
    </div>
    <Data />
    <div class="container">
      <Vaccine />
    </div>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Home from './views/Home.vue';
import Data from './components/Data.vue';
import Vaccine from './components/Vaccine.vue';

export default {
  components: {
    Navbar,
    Home,
    Data,
    Vaccine,
  },
};
</script>

<style>
body {
  font-family: 'Roboto', sans-serif;
}
.text-success {
  color: #76c893 !important;
}
</style>

<style scoped>
.home-page {
  margin-top: 100px;
  margin-bottom: 50px;
}
</style>
