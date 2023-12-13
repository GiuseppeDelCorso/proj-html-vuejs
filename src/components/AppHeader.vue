<script>

export default {
  name: "AppHeader",
}

</script>

<template>
  <div class="container">
    <div class="row my-3">
      <div class="col-6">

        <div class="dropdown">
          <button class="btn btn-secondary dropdown-toggle styleLengage" type="button" id="dropdownMenuButton2"
            data-bs-toggle="dropdown" aria-expanded="false">
            English
          </button>
          <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="dropdownMenuButton2">
            <li><a class="dropdown-item active" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
            <li>
              <hr class="dropdown-divider">
            </li>
            <li><a class="dropdown-item" href="#">Separated link</a></li>
          </ul>
        </div>
      </div>

      <div class="col-4 d-flex">
        <p class="px-2 fs-7 colorInfoText">Home</p>
        <p class="px-2 fs-7 colorInfoText">Pages</p>
        <p class="px-2 fs-7 colorInfoText">Course Formats</p>
        <p class="px-2 fs-7 colorInfoText">Course</p>
        <p class="px-2 fs-7 colorInfoText">Demos</p>
      </div>
      <div class="col-2 d-flex">
        <i class="fa-brands fa-facebook px-2 fs-7 colorInfoText"></i>
        <i class="fa-brands fa-twitter px-2 fs-7 colorInfoText"></i>
        <i class="fa-brands fa-instagram px-2 fs-7 colorInfoText"></i>
        <i class="fa-brands fa-youtube px-2 fs-7 colorInfoText"></i>
      </div>
    </div>
    <hr>
    <div class="row">
      <div class="col-2">
        <img class="imgStyle " src="../../public/img/MasterStudy.svg" alt="">
      </div>
      <div class="col-4 d-flex">
        <div class="input-group mb-4">
          <button class="btn btn-outline-secondary dropdown-toggle fs-8" type="button" data-bs-toggle="dropdown"
            aria-expanded="false"> <i class="fa-solid fa-bars pe-1"></i>CATEGORY</button>
          <ul class="dropdown-menu">

            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
            <li>
              <hr class="dropdown-divider">
            </li>
            <li><a class="dropdown-item" href="#">Separated link</a></li>
          </ul>
          <input type="text" class="form-control" placeholder="Shearch Corurses"
            aria-label="Text input with dropdown button">
        </div>
        <div class="StyleContinerShearc">
          <i class="fa-solid fa-magnifying-glass text-white mt-7"></i>
        </div>
      </div>
      <div class="col-3 d-flex">
        <div class="d-flex align-items-center">
          <i class="fa-solid fa-bullhorn fs-7 pb-3 px-2 colorInfoText"></i>
          <p class="fs-7">Beacome an Instractor</p>
        </div>
        <div class="d-flex align-items-center">
          <i class="fa-solid fa-briefcase fs-7 pb-3 px-2 ms-1 colorInfoText"></i>
          <p class="fs-7">For Enterprise</p>
        </div>
      </div>
      <div class="col-3 d-flex justify-content-end">
        <div class="d-flex align-items-center">
          <i class="fa-regular fa-user fs-7 pb-3 px-2 colorInfoText"></i>
          <p class="fs-7">Log In</p>
        </div>
        <div class="d-flex align-items-center mb-3 px-3">
          <button class="styleButton ">SIGN UP</button>
        </div>
        <div class="d-flex align-items-center mb-3 fs-4">
          <i class="fa-regular fa-heart"></i>
        </div>
      </div>
    </div>
  </div>
  <div class="container bgContainerBlack">
    <div class="row">
      <div class="col-12 d-flex justify-content-center">
        <div class="d-flex pt-3  mx-3">
          <i class="fa-solid fa-chart-simple px-2 pt-1"></i>
          <p class="fs-7">Buisness</p>
        </div>
        <div class="d-flex pt-3 mx-3">
          <i class="fa-solid fa-palette px-2 pt-1"></i>
          <p class="fs-7">Desing</p>
        </div>
        <div class="d-flex pt-3 mx-3">
          <i class="fa-solid fa-gear px-2 pt-1"></i>
          <p class="fs-7">Development</p>
        </div>
        <div class="d-flex pt-3 mx-3">
          <i class="fa-solid fa-face-smile px-2 pt-1"></i>
          <p class="fs-7">Life Style</p>
        </div>
        <div class="d-flex pt-3 mx-3">
          <i class="fa-solid fa-envelopes-bulk px-2 pt-1"></i>
          <p class="fs-7">Office Productivity</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.bgContainerBlack {
  background-color: #263144;
  color: white;
}

.styleLengage {
  background-color: white;
  color: #b3b2b3;
  border: none;
}

.colorInfoText {
  color: #b3b2b3;
}

.fs-7 {
  font-size: 14px;
}

.fs-8 {
  font-size: 10px;
}

.mt-7 {
  margin-top: 13px;
}

.imgStyle {
  height: 50px;
  width: 200px;
  object-fit: contain;
}

.StyleContinerShearc {
  text-align: center;
  background-color: #447993;
  width: 50px;
  height: 42px;

}

.styleButton {
  background-color: #ff4450;
  border: none;
  color: white;
  font-weight: bold;
  height: 50px;
  width: 90px;
  border-radius: 25px;
  font-size: 14px;
}
</style>
