<template>
  <div class="container mt-5">
    <div class="row justify-content-around">
      <div class="col-md-3 rel-bg-content rel-bg-content-left rel-rounded shadow p-4">
        <div class="rel-img-profile shadow"></div>
        <div
          class="rel-info-one text-center d-flex flex-column align-items-center justify-content-center"
        >
          <h4 class="mb-0 pb-0">Rodrigo Escobar</h4>
          <p class="mb-0 text-muted mb-2">ocralo</p>
          <div class="d-flex flex-wrap justify-content-center">
            <p class="rounded-pill rel-bg-pill p-1 m-1 btn-light shadow-sm">Web Developer</p>
          </div>
          <div class="rel-social"></div>
        </div>
        <div class="rel-info-contac d-flex flex-column mt-4">
          <div class="rel-info-contac-item d-flex p-1 text-white-50">
            <i class="far fa-calendar-alt mr-3"></i>
            <p>Julio 28, 1996</p>
          </div>
          <div class="rel-info-contac-item d-flex p-1 text-white-50">
            <i class="far fa-map mr-3"></i>
            <p>Cali, Colombia</p>
          </div>
          <div class="rel-info-contac-item d-flex p-1 text-white-50 d-inline-block text-truncate">
            <i class="far fa-envelope mr-3"></i>
            <p>
              <a href="mailto:ocralo@gmail.com" class="text-white-50">ocralo@gmail.com</a>
            </p>
          </div>
          <div class="rel-info-contac-item d-flex p-1 text-white-50">
            <i class="fas fa-mobile-alt mr-3"></i>
            <p>
              <a href="tel:+57312-866-2953" class="text-white-50">+57 (312) 866 2953</a>
            </p>
          </div>
          <div class="rel-info-contac-item d-flex p-1 text-white-50">
            <i class="fab fa-linkedin-in mr-3 mt-1"></i>
            <p>
              <a href="https://www.linkedin.com/in/ocralo/" class="text-white-50">ocralo</a>
            </p>
          </div>
        </div>
        <div class="w-100 d-flex justify-content-center mt-4">
          <a
            href="https://drive.google.com/file/d/1I1u543Xm9kp40SvonoeLGrnmaZpdM0y7/view"
            target="_blank"
            rel="noopener noreferrer"
          >
            <div class="rounded-pill text-center p-2 btn btn-primary rel-cv-download">
              <i class="fas fa-download mr-2"></i>HDV
            </div>
          </a>
        </div>
      </div>
      <div class="col-md-8 rel-bg-content rel-bg-content-rigth rel-rounded shadow mb-5">
        <div class="row d-flex justify-content-end rel-nav-sticky">
          <div class="col-md-8 bg-primary rel-nav">
            <button
              type="button"
              class="btn btn-primary h-100"
              v-if="view!=0"
              v-on:click="Changeview(0)"
            >Conoceme</button>
            <button
              type="button"
              class="btn btn-primary rel-font-bold h-100"
              v-if="view==0"
              v-on:click="Changeview(0)"
            >Conoceme</button>
            <button
              type="button"
              class="btn btn-primary h-100"
              v-if="view!=1"
              v-on:click="Changeview(1)"
            >Proyectos</button>
            <button
              type="button"
              class="btn btn-primary rel-font-bold h-100"
              v-if="view==1"
              v-on:click="Changeview(1)"
            >Proyectos</button>
            <button
              type="button"
              class="btn btn-primary h-100"
              v-if="view!=2"
              v-on:click="Changeview(2)"
            >Estudios</button>
            <button
              type="button"
              class="btn btn-primary rel-font-bold h-100"
              v-if="view==2"
              v-on:click="Changeview(2)"
            >Estudios</button>
          </div>
        </div>
        <div class="row mt-4">
          <div class="container-fluid">
            <AboutMe v-if="view==0" />
            <Proyect v-if="view==1" />
            <Estudy v-if="view==2" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AboutMe from "./AboutMe";
import Proyect from "./Proyect";
import Estudy from "./Estudy";

export default {
  name: "index",
  data() {
    return {
      view: 0
    };
  },
  components: {
    AboutMe,
    Proyect,
    Estudy
  },
  methods: {
    Changeview: function(numView) {
      this.view = numView;
    }
  }
};
</script>

<style>
.rel-bg-content {
  background: #232130;
  border-radius: 1em;
}
.rel-bg-content-left {
  max-height: 46em;
  margin-bottom: 2em;
}
.rel-bg-content-2 {
  background: #211e2b;
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
  width: 10em;
}
.rel-nav {
  border-radius: 0em 1em 0em 1em;
}

.rel-icon {
  color: #273bdd;
  font-size: 1.5em;
}

.rel-hr-title {
  background-color: #273bdd;
  height: 6px;
  border-radius: 1em;
  width: 4em;
  margin: 0em 0em 2em 0em;
}
.rel-paragraph {
  line-height: 1.3;
}

.rel-paragraph-proyect {
  line-height: 1.2;
}

.rel-item-hability {
  width: 45%;
}

.progress-bar {
  background-color: #273bdd;
}

.rel-tex-icon-proyect {
  font-size: 2em;
}

#barra-wordpress:hover:before {
  content: "50%";
}

@media (min-width: 768px) {
  .rel-bg-content-left {
    position: -webkit-sticky;
    position: sticky;
    top: 3em;
  }
}
@media (max-width: 767px) {
  .rel-nav-sticky {
    position: -webkit-sticky;
    position: sticky;
    top: 0em;
    z-index: 100;
  }
}

@media (max-width: 992px) {
  .rel-img-profile {
    margin-left: auto;
    margin-right: auto;
    height: 8em;
    width: 8em;
  }
  .rel-paragraph-proyect {
    line-height: 1.2;
    padding: 1em;
  }
}
@media (max-width: 576px) {
  .rel-img-profile {
    margin-left: auto;
    margin-right: auto;
    height: 10em;
    width: 10em;
  }
  .rel-nav {
    border-radius: 1em 1em 0em 0em;
  }
}
</style>