<template>
  <div class="vaccine mt-5 mb-5">
    <div class="row">
      <div class="col">
        <div class="kind">Kind of Vaccine</div>
      </div>
    </div>
    <div class="row mt-2">
      <div class="col">
        <div class="title">Vaccine Variant</div>
      </div>
    </div>
    <div class="row mt-3">
      <div class="col-md-3">
        <div class="card shadow">
          <div class="card-body">
            <div class="row">
              <div class="col text-center">
                <i class="bi bi-bookmarks-fill image-vaccine"></i>
              </div>
              <div class="col wrap-title">
                <h6 class="fw-bolder title-vaccine">Moderna</h6>
              </div>
            </div>
            <div class="row">
              <div class="col">
                <div class="container">
                  <div class="info-vaccine">Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt, animi?</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card shadow">
          <div class="card-body">
            <div class="row">
              <div class="col text-center">
                <i class="bi bi-bookmarks-fill image-vaccine"></i>
              </div>
              <div class="col wrap-title">
                <h6 class="fw-bolder title-vaccine">Sinovac</h6>
              </div>
            </div>
            <div class="row">
              <div class="col">
                <div class="container">
                  <div class="info-vaccine">Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt, animi?</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card shadow">
          <div class="card-body">
            <div class="row">
              <div class="col text-center">
                <i class="bi bi-bookmarks-fill image-vaccine"></i>
              </div>
              <div class="col wrap-title">
                <h6 class="fw-bolder title-vaccine">Pzifer</h6>
              </div>
            </div>
            <div class="row">
              <div class="col">
                <div class="container">
                  <div class="info-vaccine">Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt, animi?</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card shadow">
          <div class="card-body">
            <div class="row">
              <div class="col text-center">
                <i class="bi bi-bookmarks-fill image-vaccine"></i>
              </div>
              <div class="col wrap-title">
                <h6 class="fw-bolder title-vaccine">Nusantara</h6>
              </div>
            </div>
            <div class="row">
              <div class="col">
                <div class="container">
                  <div class="info-vaccine">Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt, animi?</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.kind {
  font-size: 17px;
  font-weight: bold;
  color: #76c893;
}
.title {
  font-size: 30px;
  font-weight: bolder;
}
.card {
  border: none;
  border-radius: 20px;
  height: 200px;
}
.image-vaccine {
  font-size: 50px;
  color: #76c893;
}
.wrap-title {
  display: table;
}
.title-vaccine {
  display: table-cell;
  vertical-align: middle;
  font-size: 17px;
}
.info-vaccine {
  text-align: justify;
}
</style>
