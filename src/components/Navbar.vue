<template>
  <nav class="navbar navbar-light bg-light p-2">
    <div class="container">
      <a class="navbar-brand text-center">
        <i class="bi-shield-fill-plus text-success brand">
          <span><h6 class="align-middle title">saveFromCovid</h6></span>
        </i>
      </a>
      <div class="d-flex">
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

@media only screen and (max-width: 600px) {
  .title {
    display: none;
  }
}
</style>
