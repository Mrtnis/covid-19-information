<template>
  <section class="mb-5 container-home">
    <Navbar />
    <Jumbotron />
  </section>
  <Vaccine />
  <Province />
</template>

<script>
import Navbar from '../components/Navbar.vue';
import Jumbotron from '../components/Jumbotron.vue';
import Vaccine from '../components/Vaccine.vue';
import Province from '../components/Province.vue';

export default {
  components: {
    Navbar,
    Jumbotron,
    Vaccine,
    Province,
  },
};
</script>
