<template>
  <div>
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
body {
  font-family: 'Roboto', sans-serif;
}
.text-success {
  color: #76c893 !important;
}
</style>
