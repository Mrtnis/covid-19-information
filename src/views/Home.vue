<template>
  <section>
    <!-- website -->
    <div class="home-page pb-5">
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <div class="subtitle">Get Vaccine, Boost Your Health</div>
            <div class="title">
              Get Vaccinated <br />
              Now Easly With <br />
              Vaccining.
            </div>
            <div class="information">Vaccining will help you to know your vaccine and find the nearest vaccination place from your house fast and easily to help you</div>
            <div class="row mt-4">
              <div class="col-md-8">
                <div class="btn getVaccine">Get Your Vaccine</div>
              </div>
              <div class="col-md-4">
                <div class="calendar">
                  <i class="bi bi-calendar3"></i>
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-6 image-class">
            <img src="../../public/assets/images/Home.png" class="first-image shadow" />
            <img src="../../public/assets/images/Details.png" class="second-image shadow" />
          </div>
        </div>
      </div>
    </div>
    <!-- mobile -->
    <div class="mobile-page pb-5">
      <div class="container">
        <div class="row mt-5">
          <div class="col-md image-mobile">
            <img src="../../public/assets/images/Home.png" class="first-mobile shadow" />
            <img src="../../public/assets/images/Details.png" class="second-mobile shadow" />
          </div>
        </div>
        <div class="row">
          <div class="col">
            <div class="subtitle">Get Vaccine, Boost Your Health</div>
            <div class="title">Get Vaccinated Now Easly With Vaccining.</div>
            <div class="information">Vaccining will help you to know your vaccine and find the nearest vaccination place from your house fast and easily to help you</div>
            <div class="row mt-4 mobile-wrap">
              <div class="col-8">
                <div class="btn getVaccine">Get Your Vaccine</div>
              </div>
              <div class="col-4">
                <div class="calendar">
                  <i class="bi bi-calendar3"></i>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Data from './../components/Data.vue';
import Province from './../components/Province.vue';

export default {
  components: {
    Data,
    Province,
  },
};
</script>

<style>
.medicine {
  height: 100%;
  width: 100%;
}
.subtitle {
  color: #17bfe9;
  margin-bottom: 20px;
}
.title {
  font-size: 45px;
  font-weight: bolder;
  color: #fff;
}
.getVaccine {
  color: white;
  border: none;
  border-radius: 20px;
  padding: 25px;
  padding-right: 90px;
  padding-left: 90px;
  background: linear-gradient(to right, rgba(255, 255, 255, 0.15) 50%, #17bfe9 50%);
  background-size: 200% 100%;
  background-position: right bottom;
  transition: all 0.5s ease-out;
  font-weight: bolder;
  font-size: 20px;
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
  background: linear-gradient(to right, rgba(255, 255, 255, 0.15) 50%, #17bfe9 50%);
  background-size: 200% 100%;
  background-position: left bottom;
  transition: all 0.3s ease-out;
  font-size: 20px;
  color: #17bfe9;
}
.calendar:hover {
  background-position: right bottom;
  color: white;
  cursor: pointer;
}
.bi-calendar3 {
  line-height: 70px;
  font-size: 30px;
}
.home-page {
  margin-top: 50px;
}
.image-class {
  display: flex;
  align-items: center;
  position: relative;
}
.first-image,
.second-image {
  width: 200px;
  border-radius: 20px;
}
.first-image {
  transform: rotate(-5deg);
  z-index: 2;
  margin-top: -40px;
  margin-right: -15px;
}
.second-image {
  transform: rotate(5deg);
}

@media only screen and (min-width: 768px) {
  .image-class:hover .first-image,
  .image-class:hover .second-image {
    transition: 0.3s ease;
    transform: rotate(0deg);
  }
  .image-class:hover .first-image {
    transition: 0.3s ease;
    margin-right: 15px;
  }
  .mobile-page {
    display: none;
  }
  .information {
    margin-top: 30px;
    width: 70%;
    color: #8289b2;
    font-weight: 10px;
  }
}

@media only screen and (max-width: 600px) {
  .home-page {
    display: none;
  }
  .image-mobile {
    display: flex;
    align-items: center;
    position: relative;
    justify-content: center;
    margin-bottom: 40px;
  }
  .first-mobile,
  .second-mobile {
    width: 150px;
    border-radius: 20px;
  }
  .first-mobile {
    transform: rotate(-5deg);
    z-index: 2;
    margin-top: -40px;
    margin-right: -15px;
  }
  .second-mobile {
    transform: rotate(5deg);
  }
  .subtitle {
    text-align: center;
  }
  .title {
    text-align: center;
    font-size: 30px;
  }
  .information {
    margin-top: 30px;
    color: #8289b2;
    font-weight: 10px;
    text-align: center;
  }
  .mobile-wrap {
    display: flex;
    align-items: center;
  }
  .getVaccine {
    font-size: 18px;
    padding: 30px;
  }
}
</style>
