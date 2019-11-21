<template>
  <div class="container mt-5">
    <div class="row justify-content-around">
      <div class="col-md-3 rel-bg-content rel-rounded shadow p-4">
        <div class="rel-img-profile shadow"></div>
        <div
          class="rel-info-one text-center d-flex flex-column align-items-center justify-content-center"
        >
          <h4 class="mb-0 pb-0">Rodrigo Escobar</h4>
          <p class="mb-0 text-muted mb-2">ocralo</p>
          <p class="rounded-pill rel-bg-pill p-1 m-1 btn-light shadow-sm">Game Developer</p>
          <p class="rounded-pill rel-bg-pill p-1 m-1 btn-light shadow-sm">Web Developer</p>
          <div class="rel-social"></div>
        </div>
        <div class="rel-info-contac d-flex flex-column mt-4">
          <div class="rel-info-contac-item d-flex p-1 text-white-50">
            <i class="far fa-calendar-alt mr-3"></i>
            <p>Julio 21, 1996</p>
          </div>
          <div class="rel-info-contac-item d-flex p-1 text-white-50">
            <i class="far fa-map mr-3"></i>
            <p>Cali, Colombia</p>
          </div>
          <div class="rel-info-contac-item d-flex p-1 text-white-50 d-inline-block text-truncate">
            <i class="far fa-envelope mr-3"></i>
            <p>ocralo@gmail.com</p>
          </div>
          <div class="rel-info-contac-item d-flex p-1 text-white-50">
            <i class="fas fa-mobile-alt mr-3"></i>
            <p>+57 (312) 866 2953</p>
          </div>
          <div class="rel-info-contac-item d-flex p-1 text-white-50">
            <i class="fab fa-linkedin-in mr-3 mt-1"></i>
            <p>ocralo</p>
          </div>
        </div>
        <div class="w-100 d-flex justify-content-center mt-4">
          <div class="rel-cv-download rounded-pill text-center p-2 btn btn-primary">
            <i class="fas fa-download mr-2"></i>HDV
          </div>
        </div>
      </div>
      <div class="col-md-8 rel-bg-content rel-rounded shadow">
        <div class="row justify-content-around">
          <div class="col-md-3">
            <h4>Conoceme</h4>
          </div>
          <div class="col-md-9 bg-primary rel-nav">
            <button type="button" class="btn btn-primary">Conoceme</button>
            <button type="button" class="btn btn-primary">Proyectos</button>
            <button type="button" class="btn btn-primary">Habilidades</button>
            <button type="button" class="btn btn-primary">Estudios</button>
            <button type="button" class="btn btn-primary">Certificados</button>
          </div>
        </div>
        <div class="row">
          <div class="container-fluid">
            <div class="row"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.rel-bg-content {
  background: #232130;
  border-radius: 1em;
}
.rel-img-profile {
  background-image: url("~@/assets/img/Rodrigo.jpg");
  position: relative;
  top: -3em;
  margin-left: auto;
  margin-right: auto;
  height: 10em;
  width: 10em;
  border-radius: 1em;
  background-color: #cccccc;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.rel-bg-pill {
  background: #1d1a25;
  font-size: 12px;
  color: #ffffff !important;
  width: 12em;
}
.rel-bg-pill:hover {
  color: #1d1a25 !important;
}
.rel-cv-download {
  width: 18em;
}
.rel-nav {
  border-radius: 0 1em 0em 1em;
}

@media (max-width: 992px) {
  .rel-img-profile {
    margin-left: auto;
    margin-right: auto;
    height: 8em;
    width: 8em;
  }
}
@media (max-width: 576px) {
  .rel-img-profile {
    margin-left: auto;
    margin-right: auto;
    height: 10em;
    width: 10em;
  }
}
</style>