<template>
  <div class="home">
    <div class="row">
      <div class="col-md-6">
        <div class="tagline">
          Let's <span class="tag">protect</span> <br />
          each other from <span class="tag">covid.</span>
        </div>
        <div class="information">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quibusdam, voluptas sint. Obcaecati alias quis esse suscipit, voluptates officiis nulla soluta.</div>
        <div class="row mt-4">
          <div class="col-md">
            <div class="btn getVaccine">Get Your Vaccine</div>
          </div>
          <div class="col-md">
            <div class="btn learnMore">Learn More</div>
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
  background-color: #76c893;
  color: white;
  border-radius: 30px;
  padding: 15px;
  padding-right: 40px;
  padding-left: 40px;
  box-shadow: 0 10px 18px #76c893;
}
.learnMore {
  border-color: #76c893;
  border-radius: 30px;
  color: #76c893;
  padding: 15px;
  padding-right: 50px;
  padding-left: 50px;
}
</style>
