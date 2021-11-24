<template>
  <div class="container my-5">
    <!-- title -->
    <div class="subtitle mb-2">Location</div>
    <div class="flex-title mb-3">
      <div class="title">Get Vaccine Location</div>
      <div class="flex-arrow">
        <i class="bi bi-caret-left-fill"></i>
        <i class="bi bi-caret-right-fill"></i>
      </div>
    </div>
    <!-- location -->
    <div class="flex-location">
      <div class="col-md-3">
        <div class="card border">
          <div class="card-header" style="background-image: url('https://picsum.photos/id/234/300')"></div>
          <div class="card-body">
            <div class="title-loc">White Square</div>
            <div class="subtitle-loc">Lorem ipsum dolor sit amet consectetur.</div>
            <div class="flex-button">
              <div class="btn btn-sm button-loc">Select location</div>
              <i class="bi bi-calendar-fill"></i>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card border">
          <div class="card-header" style="background-image: url('https://picsum.photos/id/24/300')"></div>
          <div class="card-body">
            <div class="title-loc">White Square</div>
            <div class="subtitle-loc">Lorem ipsum dolor sit amet consectetur.</div>
            <div class="flex-button">
              <div class="btn btn-sm button-loc">Select location</div>
              <i class="bi bi-calendar-fill"></i>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card border">
          <div class="card-header" style="background-image: url('https://picsum.photos/id/22/300')"></div>
          <div class="card-body">
            <div class="title-loc">White Square</div>
            <div class="subtitle-loc">Lorem ipsum dolor sit amet consectetur.</div>
            <div class="flex-button">
              <div class="btn btn-sm button-loc">Select location</div>
              <i class="bi bi-calendar-fill"></i>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card border">
          <div class="card-header" style="background-image: url('https://picsum.photos/id/114/300')"></div>
          <div class="card-body">
            <div class="title-loc">White Square</div>
            <div class="subtitle-loc">Lorem ipsum dolor sit amet consectetur.</div>
            <div class="flex-button">
              <div class="btn btn-sm button-loc">Select location</div>
              <i class="bi bi-calendar-fill"></i>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card border">
          <div class="card-header" style="background-image: url('https://picsum.photos/id/187/300')"></div>
          <div class="card-body">
            <div class="title-loc">White Square</div>
            <div class="subtitle-loc">Lorem ipsum dolor sit amet consectetur.</div>
            <div class="flex-button">
              <div class="btn btn-sm button-loc">Select location</div>
              <i class="bi bi-calendar-fill"></i>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
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
.bi-caret-left-fill {
  padding: 7px;
  color: #b9c3d9;
  border-radius: 50%;
  margin-right: 20px;
  background-color: #f2f2f4;
}
.bi-caret-right-fill {
  padding: 7px;
  color: #fff;
  border-radius: 50%;
  background-color: var(--secondary-color);
}
.flex-location {
  display: flex;
  overflow-x: auto;
  margin-bottom: 20px;
}
.flex-location::-webkit-scrollbar {
  display: none;
}
.card {
  border: none;
  margin-right: 20px;
  border-radius: 10px;
}
.card-header {
  height: 180px;
  border-start-end-radius: 10px;
  border-start-start-radius: 10px;
}
.title-loc {
  font-size: 20px;
  font-weight: bolder;
  color: var(--primary-color);
}
.subtitle-loc {
  font-size: 12px;
  font-weight: bold;
  text-align: start;
  color: #b9c3d9;
}
.flex-button {
  display: flex;
  margin-top: 20px;
  align-items: center;
}
.button-loc {
  color: #fff;
  margin-right: 30px;
  padding-left: 20px;
  border-radius: 10px;
  padding-right: 20px;
  background-color: var(--secondary-color);
}
.bi-calendar-fill {
  font-size: 20px;
  color: var(--secondary-color);
}
</style>
