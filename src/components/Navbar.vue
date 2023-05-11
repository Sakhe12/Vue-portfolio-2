<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container-fluid">
          <a class="navbar-brand" href="/">Sakhe Mzolisa</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ms-auto mb-2 mb-lg-0 text-light gap-3">
                <li class="nav-item">
                    <router-link class="txt-col" to="/">Home</router-link>
                </li>
                <li class="nav-item">
                    <router-link class="txt-col" to="/about">About</router-link>
                </li>
                <li class="nav-item">
                    <router-link class="txt-col" to="/resume">Resume</router-link>
                </li>
                <li class="nav-item">
                    <router-link class="txt-col" to="/projects">Projects</router-link>
                </li>
                <li class="nav-item">
                    <router-link class="txt-col" to="/testimonials">Testimonial</router-link>
                </li>
                <li class="nav-item">
                    <router-link class="txt-col" to="/contact">Contact</router-link>
                </li>
            </ul>
          </div>
        </div>
      </nav>
</template>
<script>
export default {
    
}
</script>
<style >
.txt-col {
    text-decoration: none;
    color: black;
    transition:col 0.6s;
}
.txt-col:hover {
    color: #fff;
    text-shadow: 0 0 10px #fff,
                 0 0 10px #fff,
                 0 0 10px #fff,
                 0 0 10px #fff;
 }
.fa-solid {
    color: aqua;
}
.txt-col :hover {
    color: #fff;
    text-shadow: 0 0 10px #fff,
                 0 0 10px #fff,
                 0 0 10px #fff,
                 0 0 10px #fff;
 }

</style>