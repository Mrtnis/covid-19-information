<template>
  <div class="container">
    <!-- title -->
    <div class="subtitle mb-2">Kind of Vaccine</div>
    <div class="flex-title mb-3">
      <div class="title">Vaccine Variant</div>
      <div class="flex-arrow">
        <i class="bi bi-caret-left-fill"></i>
        <i class="bi bi-caret-right-fill"></i>
      </div>
    </div>
    <!-- variant -->
    <div class="flex-variant">
      <div class="col-md-4">
        <div class="card border">
          <div class="card-body">
            <div class="flex-icon">
              <i class="bi bi-hourglass-split"></i>
              <div class="title-icon">Moderna</div>
            </div>
            <div class="info-icon">Lorem ipsum dolor sit amet consectetur adipisicing elit</div>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card border card-active">
          <div class="card-body">
            <div class="flex-icon">
              <i class="bi bi-hourglass-split icon-active"></i>
              <div class="title-icon text-active">Sinnovac</div>
            </div>
            <div class="info-icon text-active">Lorem ipsum dolor sit amet consectetur adipisicing elit</div>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card border">
          <div class="card-body">
            <div class="flex-icon">
              <i class="bi bi-hourglass-split"></i>
              <div class="title-icon">Pfizer</div>
            </div>
            <div class="info-icon">Lorem ipsum dolor sit amet consectetur adipisicing elit</div>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card border">
          <div class="card-body">
            <div class="flex-icon">
              <i class="bi bi-hourglass-split"></i>
              <div class="title-icon">Astra Zeneca</div>
            </div>
            <div class="info-icon">Lorem ipsum dolor sit amet consectetur adipisicing elit</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  color: #fbfdff;
}
.subtitle {
  font-weight: bold;
  text-align: start;
  color: var(--secondary-color);
}
.flex-title {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.title {
  font-size: 35px;
  font-weight: bolder;
  color: var(--primary-color);
}
.bi-caret-left-fill,
.bi-caret-right-fill {
  font-size: 35px;
}
.bi-caret-left-fill {
  color: #ced6ec;
}
.bi-caret-right-fill {
  color: var(--secondary-color);
}
.flex-variant {
  display: flex;
  overflow-x: auto;
  margin-bottom: 20px;
}
.flex-variant::-webkit-scrollbar {
  display: none;
}
.card {
  border: none;
  padding: 10px;
  height: 180px;
  margin-right: 20px;
  border-radius: 10px;
  margin-bottom: 20px;
}
.flex-icon {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}
.flex-icon i {
  padding-top: 5px;
  margin-right: 10px;
  padding-left: 10px;
  padding-right: 10px;
  border-radius: 10px;
  padding-bottom: 5px;
  background-color: #e8f7fb;
  color: var(--secondary-color);
}
.title-icon {
  font-size: 18px;
  font-weight: bolder;
  color: var(--primary-color);
}
.info-icon {
  padding: 5px;
  color: #8289b2;
  text-align: start;
}
.card-active {
  background-color: var(--primary-color);
}
.text-active {
  color: #fff;
}
.icon-active {
  color: #fff !important;
  background-color: var(--secondary-color) !important;
}
</style>
