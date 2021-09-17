<template>
  <div class="container">
    <div class="card">
      <div class="card-body">
        <div class="row text-center">
          <div class="col text-danger">
            <div class="title">204</div>
            <div class="subtitle">Affected Country</div>
          </div>
          <div class="col text-danger">
            <div class="title">1,098,848</div>
            <div class="subtitle">Confirmed Cases</div>
          </div>
          <div class="col text-success">
            <div class="title">226.106</div>
            <div class="subtitle">Recover Cases</div>
          </div>
          <div class="col text-danger">
            <div class="title">58,871</div>
            <div class="subtitle">Worlwide Death</div>
          </div>
        </div>
        <div class="row mt-4">
          <div class="col">
            <div class="text-center info">
              See all data covid in Indonesian.
              <span @click="getData" class="text-success source">Klik here!</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios';

export default {
  data() {
    return {
      data: '',
    };
  },
  methods: {
    getData() {
      axios.get('https://covid19.mathdro.id/api').then(({ data }) => {
        console.log(data);
      });
    },
  },
};
</script>

<style scoped>
.card {
  border-radius: 20px;
  padding: 10px;
  border: none;
  box-shadow: inset 0px 0px 10px #76c893;
}
.title {
  font-size: 35px;
  font-weight: bold;
}
.info {
  color: gray;
  font-size: 15px;
}
.source {
  border-bottom: 1px solid #76c893;
  cursor: pointer;
}
</style>
