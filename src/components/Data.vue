<template>
  <div class="container">
    <div class="card">
      <div class="card-body">
        <div class="row text-center">
          <div class="col-md-3 col-xs-12 text-success">
            <div class="title">{{ data.length - 1 }}</div>
            <div class="subtitle">Data Province</div>
            <hr class="line-cases" />
          </div>
          <div class="col-md-3 col-xs-12 text-danger">
            <div class="title">{{ formatNumber(countPositive) }}</div>
            <div class="subtitle">Positive Cases</div>
            <hr class="line-cases" />
          </div>
          <div class="col-md-3 col-xs-12 text-success">
            <div class="title">{{ formatNumber(countRecovery) }}</div>
            <div class="subtitle">Recover Cases</div>
            <hr class="line-cases" />
          </div>
          <div class="col-md-3 col-xs-12 text-danger">
            <div class="title">{{ formatNumber(countDeath) }}</div>
            <div class="subtitle">Death Cases</div>
            <hr class="line-cases" />
          </div>
        </div>
        <div class="row mt-4">
          <div class="col">
            <div class="text-center info">
              Data get from
              <span><a href="https://indonesia-covid-19.mathdro.id" class="text-success source">https://indonesia-covid-19.mathdro.id</a></span>
            </div>
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
      data: [],
      api_origin: api.API_ORIGIN,
    };
  },
  methods: {
    formatNumber(par) {
      return new Intl.NumberFormat().format(par);
    },
  },
  computed: {
    countPositive() {
      return this.data.reduce(function (item, dt) {
        return item + dt.kasusPosi;
      }, 0);
    },
    countRecovery() {
      return this.data.reduce(function (item, dt) {
        return item + dt.kasusSemb;
      }, 0);
    },
    countDeath() {
      return this.data.reduce(function (item, dt) {
        return item + dt.kasusMeni;
      }, 0);
    },
  },
  mounted() {
    axios.get(`${this.api_origin}/api/provinsi/`).then(({ data }) => {
      this.data = data.data;
    });
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
a {
  text-decoration: none;
}
@media only screen and (max-width: 600px) {
  .col-xs-12 {
    margin-bottom: 30px;
  }
  .line-cases {
    margin-top: 10px !important;
    margin: auto;
    width: 60%;
  }
}

@media only screen and (min-width: 600px) {
  .line-cases {
    display: none;
  }
}
</style>
