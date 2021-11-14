<template>
  <div class="landing-page">
    <Navbar />
    <router-view></router-view>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';

export default {
  components: {
    Navbar,
  },
};
</script>

<style>
* {
  --primary-color: #060c23;
}
body {
  font-family: 'Roboto', sans-serif;
}
.landing-page {
  background-color: var(--primary-color);
}
.text-success {
  color: #76c893 !important;
}
</style>
