<template>
  <nav class="navbar navbar-light p-2">
    <div class="container">
      <a class="navbar-brand text-center">
        <i class="bi-shield-fill-plus text-success brand"> </i>
        <span
          ><h6 class="align-middle title fw-bolder">saveFromCovid<span class="text-dark">.go.id</span></h6></span
        >
      </a>
      <div class="d-flex d-md-block d-none">
        <div class="row">
          <div class="col">
            <h6 class="active">Home</h6>
          </div>
          <div class="col">
            <h6>About</h6>
          </div>
          <div class="col">
            <h6>Variant</h6>
          </div>
          <div class="col">
            <h6>Vaccine</h6>
          </div>
          <div class="col">
            <h6 class="contact">Contact</h6>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.brand {
  font-size: 2rem;
}
.active {
  border-bottom: 2px solid #76c893;
  color: black;
}
.d-flex {
  color: #76c893;
}
.contact {
  background-color: #76c893;
  color: white;
  border-radius: 25px;
  text-align: center;
  padding-right: 20px;
  padding-left: 20px;
  padding-top: 5px;
  padding-bottom: 5px;
  margin-top: -5px;
}
.title {
  color: #76c893;
}

@media only screen and (max-width: 600px) {
  .title {
    display: none;
  }
}
</style>
