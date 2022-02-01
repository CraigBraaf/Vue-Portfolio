<template>
  <div class="navy">
      <nav class="navbar navbar-expand-lg navbar-dark bg-transparent">

  <div class="container-fluid">
    <button
      class="navbar-toggler"
      type="button"
      data-mdb-toggle="collapse"
      data-mdb-target="#navbarRightAlignExample"
      aria-controls="navbarRightAlignExample"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <i class="fas fa-bars"></i>
    </button>


    <div class="collapse navbar-collapse" id="navbarRightAlignExample">
      <ul class="navbar-nav ms-auto mb-2 mb-lg-2">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link active" href="#About">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link active" href="#Skills">Skills</a>
        </li>
        <li class="nav-item">
          <a class="nav-link active" href="#Projects">Projects</a>
        </li>
         <li class="nav-item">
          <a class="nav-link active" href="#Testimonials">Testimonials</a>
        </li>
         <li class="nav-item">
          <a class="nav-link active" href="#Contact">Contact Me</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
      </div>
</template>

<script>
export default {


}
</script>

<style>
.navy {

    position: fixed;
    top: 0;
    width: 100%;
}

.nav-item {
  display: inline-block;
  position: relative;
  color: #000000;
}

.nav-item:after {
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 2px;
  bottom: 0;
  left: 0;
  background-color: #ffffff;
  transform-origin: bottom right;
  transition: transform 0.25s ease-out;
}

.nav-item:hover:after {
      transform: scaleX(1);
  transform-origin: bottom left;
}
</style>