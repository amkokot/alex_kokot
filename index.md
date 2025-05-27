---
layout: main
title: "Home"
permalink: /
---

<!-- Two-column intro + carousel -->
<div class="intro-carousel-container">
  <!-- Left column: photo, name, intro -->
  <div class="intro-col">
    <img 
      src="{{ site.baseurl }}/assets/images/alex_kokot.jpg" 
      alt="Alex Kokot" 
      class="intro-photo"
    />
    <h2>Alex Kokot</h2>
    <p>
      I’m a PhD student in the Department of Statistics at the University of Washington.  
      My research focuses on kernel methods, optimal transport, and applications of ML to scientific data.
    </p>
  </div>

  <!-- Right column: carousel -->
  <div class="carousel-col">
    <div id="researchCarousel" class="carousel slide carousel-fade mb-4" data-bs-ride="carousel">
      <!-- Indicators -->
      <div class="carousel-indicators">
        <button type="button" data-bs-target="#researchCarousel" data-bs-slide-to="0" class="active"></button>
        <button type="button" data-bs-target="#researchCarousel" data-bs-slide-to="1"></button>
        <button type="button" data-bs-target="#researchCarousel" data-bs-slide-to="2"></button>
        <button type="button" data-bs-target="#researchCarousel" data-bs-slide-to="3"></button>
        <button type="button" data-bs-target="#researchCarousel" data-bs-slide-to="4"></button>
      </div>

      <!-- Slides -->
      <div class="carousel-inner">
        <div class="carousel-item active" data-caption="Treemap visualization on MNIST embeddings">
          <img
            src="{{ site.baseurl }}/assets/images/mnist_treemap.png"
            class="d-block"
            alt="MNIST Treemap"
          />
        </div>
        <div class="carousel-item" data-caption="Categorical scatter of MNIST">
          <img
            src="{{ site.baseurl }}/assets/images/mnist_scatter_categorical.png"
            class="d-block"
            alt="MNIST Scatter"
          />
        </div>
        <div class="carousel-item" data-caption="Wide Gauss grid demonstration">
          <img
            src="{{ site.baseurl }}/assets/images/gauss_grid_wide.png"
            class="d-block"
            alt="Gauss Grid"
          />
        </div>
        <div class="carousel-item" data-caption="Sasaki divergence comparison">
          <img
            src="{{ site.baseurl }}/assets/images/sasaki.png"
            class="d-block"
            alt="Sasaki Plot"
          />
        </div>
        <div class="carousel-item" data-caption="Clean vs noisy data example">
          <img
            src="{{ site.baseurl }}/assets/images/clean_vs_noisy.png"
            class="d-block"
            alt="Clean vs Noisy"
          />
        </div>
      </div>

      <!-- Prev/Next controls -->
      <button class="carousel-control-prev" type="button"
              data-bs-target="#researchCarousel" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button class="carousel-control-next" type="button"
              data-bs-target="#researchCarousel" data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>

    <!-- Caption below the frame -->
    <div id="carouselCaption" class="text-center text-dark mt-2"></div>
  </div>
</div>

<!-- Initialize caption switching -->
<script>
  document.addEventListener('DOMContentLoaded', function() {
    const carousel = document.getElementById('researchCarousel');
    const caption = document.getElementById('carouselCaption');

    function updateCaption() {
      const active = carousel.querySelector('.carousel-item.active');
      caption.textContent = active.getAttribute('data-caption') || '';
    }

    carousel.addEventListener('slid.bs.carousel', updateCaption);
    updateCaption();
  });
</script>

<!-- (rest of your Home page content…) -->
