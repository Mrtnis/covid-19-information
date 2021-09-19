<template>
  <section>
    <!-- website -->
    <div class="home-page d-md-block d-none">
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <div class="tagline">
              Let's <span class="tag">protect</span> <br />
              each other from <span class="tag">covid.</span>
            </div>
            <div class="information">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quibusdam, voluptas sint. Obcaecati alias quis esse suscipit, voluptates officiis nulla soluta.</div>
            <div class="row mt-4">
              <div class="col-md-8">
                <div class="btn getVaccine">Get Your Vaccine</div>
              </div>
              <div class="col-md-4">
                <div class="calendar">
                  <i class="bi bi-calendar-check-fill"></i>
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-6 image-class">
            <lord-icon src="https://cdn.lordicon.com/hsotfjpx.json" stroke="30" trigger="loop-on-hover" colors="primary:#121331,secondary:#08a88a" class="medicine"> </lord-icon>
          </div>
        </div>
      </div>
    </div>
    <!-- mobile -->
    <div class="d-sm-block d-md-none mt-3">
      <div class="container">
        <div class="row">
          <div class="col">
            <div class="tagline text-center">
              Let's <span class="tag">protect</span> <br />
              each other from <span class="tag">covid.</span>
            </div>
          </div>
        </div>
        <div class="row mt-4">
          <div class="col-md-6 image-class">
            <lord-icon src="https://cdn.lordicon.com/hsotfjpx.json" stroke="30" trigger="hover" colors="primary:#121331,secondary:#08a88a" class="medicine"> </lord-icon>
          </div>
        </div>
        <div class="row">
          <div class="col">
            <div class="information">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quibusdam, voluptas sint. Obcaecati alias quis esse suscipit, voluptates officiis nulla soluta.</div>
          </div>
        </div>
        <div class="container">
          <div class="row mobile-button">
            <div class="btn getVaccine">Get Your Vaccine</div>
            <div class="calendar">
              <i class="bi bi-calendar-check-fill"></i>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Data -->
    <Data />
    <!-- vaccine -->
    <div class="container">
      <Vaccine />
    </div>
  </section>
</template>

<script>
import Data from './../components/Data.vue';
import Vaccine from './../components/Vaccine.vue';

export default {
  components: {
    Data,
    Vaccine,
  },
};
</script>

<style>
.image-class {
  margin-top: -100px;
}
.medicine {
  height: 100%;
  width: 100%;
}
.tagline {
  font-size: 45px;
  font-weight: 900;
}
.tag {
  color: #76c893;
}
.information {
  margin-top: 30px;
  width: 80%;
  text-align: justify;
  color: rgb(70, 69, 69);
  letter-spacing: 2px;
  line-height: 30px;
}
.getVaccine {
  color: white;
  border: none;
  border-radius: 20px;
  padding: 25px;
  padding-right: 90px;
  padding-left: 90px;
  background: linear-gradient(to right, #d9534f 50%, #76c893 50%);
  background-size: 200% 100%;
  background-position: right bottom;
  transition: all 0.5s ease-out;
}
.getVaccine:hover {
  background-position: left bottom;
  color: white;
}
.calendar {
  text-align: center;
  height: 70px;
  width: 70px;
  border-radius: 50%;
  background: linear-gradient(to left, #d9534f 50%, #76c893 50%);
  background-size: 200% 100%;
  background-position: left bottom;
  transition: all 0.5s ease-out;
}
.calendar:hover {
  background-position: right bottom;
  color: white;
}
.bi-calendar-check-fill {
  color: white;
  line-height: 70px;
  font-size: 30px;
}
.home-page {
  margin-top: 100px;
}

@media only screen and (max-width: 600px) {
  .tagline {
    font-size: 35px;
    font-weight: 900;
    margin-bottom: 40px;
  }
  .medicine {
    height: 90%;
    width: 90%;
  }
  .image-class {
    text-align: center;
  }
  .information {
    text-align: center;
    width: auto;
    margin-top: -50px;
    margin-bottom: 30px;
  }
  .mobile-button {
    display: grid;
    grid-template-columns: auto auto auto;
    margin-bottom: 40px !important;
    justify-content: space-evenly;
    margin: auto;
  }
  .getVaccine {
    padding-right: 70px;
    padding-left: 70px;
  }
}
</style>
