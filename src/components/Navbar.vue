<template>
  <nav class="navbar navbar-light p-2 pt-4">
    <div class="container">
      <a class="navbar-brand text-center">
        <div class="title">Vaccining</div>
      </a>
      <div class="row nav-center">
        <div class="col">
          <p class="active">Home</p>
        </div>
        <div class="col">
          <p>Features</p>
        </div>
        <div class="col">
          <p>Schedule</p>
        </div>
        <div class="col">
          <p>Quota</p>
        </div>
        <div class="col">
          <p>Contact</p>
        </div>
      </div>
      <div>
        <div class="row">
          <div class="col">
            <h6 class="get-vaccine">Call Center</h6>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.nav-center {
  color: #5d6581;
  font-weight: 600;
}
.get-vaccine {
  color: #17bfe9;
  padding: 15px;
  border-radius: 10px;
  font-weight: bolder;
  background: linear-gradient(to right, rgba(255, 255, 255, 0.15) 50%, #17bfe9 50%);
  background-size: 200% 100%;
  background-position: left bottom;
  transition: all 0.5s ease-out;
}
.get-vaccine:hover {
  background-position: right bottom;
  cursor: pointer;
  color: #fff;
}
.title {
  color: #fff;
  font-size: 25px;
  font-weight: bolder;
}
.active {
  color: #fff;
  position: relative;
}
.active::after {
  content: '';
  position: absolute;
  width: 5px;
  height: 5px;
  background-color: #17bfe9;
  border-radius: 50%;
  bottom: -10px;
  left: 0;
  right: 0;
  margin-left: auto;
  margin-right: auto;
}

@media only screen and (max-width: 600px) {
  .bi-list {
    font-size: 25px;
  }
  .nav-center {
    display: none;
  }
}
</style>
