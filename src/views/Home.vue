<template>
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
      <div class="col-md-6">
        <img src="../../public/assets/images/medicine.svg" alt="medicine" class="medicine" />
      </div>
    </div>
  </div>
</template>

<style>
.medicine {
  height: 100%;
  width: 100%;
  transition: width 2s ease;
}
.medicine:hover {
  width: 80%;
  align-content: center !important;
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
  background-color: #76c893;
}
.bi-calendar-check-fill {
  color: white;
  line-height: 70px;
  font-size: 30px;
}
</style>
