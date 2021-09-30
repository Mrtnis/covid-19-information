<template>
  <div class="container mt-5 mb-5">
    <div class="row">
      <div class="col">
        <div class="mb-3 title">Data By <span>Province</span></div>
      </div>
    </div>
    <div class="row justify-content-center mb-3">
      <div class="col-md-6">
        <div class="input-group mb-3">
          <span class="input-group-text"><i class="bi bi-search text-light"></i></span>
          <input v-model="search" type="text" class="form-control" placeholder="Search Province..." />
        </div>
      </div>
    </div>
    <div v-if="countData">
      <div class="row">
        <div class="col text-center">
          <div class="text-danger">Uupss, province is not found. Please check your input :(</div>
        </div>
      </div>
    </div>
    <div class="image-scroll">
      <div class="card" style="width: 18rem" v-for="(data, index) in searchProvince" :key="index">
        <div>
          <img :src="image + data.provinsi + '.png'" class="card-img-top" />
          <div class="card-body">
            <div class="fw-bolder h5">{{ data.provinsi }}</div>
            <h6>Positive Cases: {{ formatNumber(data.kasusPosi) }}</h6>
            <h6>Recover Cases: {{ formatNumber(data.kasusSemb) }}</h6>
            <h6>Death Cases: {{ formatNumber(data.kasusMeni) }}</h6>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios';
import api from '../api';

export default {
  data() {
    return {
      allData: [],
      search: '',
      api_origin: api.API_ORIGIN,
      image: 'public/assets/images/province/',
    };
  },
  methods: {
    formatNumber(par) {
      return new Intl.NumberFormat().format(par);
    },
  },
  computed: {
    filteredProvinces() {
      return this.allData.filter((item) => {
        return item.provinsi !== 'Indonesia';
      });
    },
    searchProvince() {
      return this.filteredProvinces.filter((item) => {
        return item.provinsi.toLowerCase().includes(this.search.toLowerCase());
      });
    },
    countData() {
      return this.searchProvince.length === 0 ? true : false;
    },
  },
  mounted() {
    axios.get(`${this.api_origin}/api/provinsi/`).then(({ data }) => {
      this.allData = data.data;
    });
  },
};
</script>

<style scoped>
.title {
  font-size: 35px;
  font-weight: 900;
  text-align: center;
}
.title span {
  color: #76c893;
}
.image-scroll {
  display: flex;
  flex-wrap: no-wrap;
  overflow-x: auto;
}
.card {
  flex: 0 0 auto;
  margin-right: 15px;
  border-radius: 20px;
  background-color: #76c893;
  border: none;
  color: white;
}
.card-img-top {
  border-top-left-radius: 20px;
  border-top-right-radius: 20px;
}
.input-group-text {
  background-color: #76c893;
}
::-webkit-scrollbar {
  height: 0;
  width: 0;
}
</style>
