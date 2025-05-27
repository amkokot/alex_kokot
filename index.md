---
layout: main
title: "Home"
permalink: /
---

<!-- Simple inline intro -->
<div class="intro-inline">
  <img 
    src="{{ site.baseurl }}/assets/images/alex_kokot.jpg" 
    alt="Alex Kokot" 
    class="intro-img"
  />
  <div class="intro-text">
    <h2>Alex Kokot, University of Washington</h2>
    <p>
      I’m a PhD student in the Department of Statistics at the University of Washington.  
      My research focuses on kernel methods, optimal transport, and ML for scientific data.
    </p>
  </div>
</div>

<!-- Carousel component (Bootstrap) -->
<div id="researchCarousel" class="carousel slide mb-4" data-bs-ride="carousel">
  <!-- Slides -->
  <div class="carousel-inner">
    <div class="carousel-item active" data-caption="Treemap visualization of a Sinkhorn coreset of MNIST data from https://arxiv.org/abs/2504.20194">
      <img src="{{ site.baseurl }}/assets/images/mnist_treemap.png"
           class="d-block w-100"
           alt="Research Figure 1">
    </div>
    <div class="carousel-item" data-caption="Geometric visualization of a Sinkhorn coreset of MNIST data from https://arxiv.org/abs/2504.20194">
      <img src="{{ site.baseurl }}/assets/images/mnist_scatter_categorical.png"
           class="d-block w-100"
           alt="Research Figure 2">
    </div>
    <div class="carousel-item" data-caption="Sinkhorn coreset from a Gaussian mixture from https://arxiv.org/abs/2504.20194">
      <img src="{{ site.baseurl }}/assets/images/gauss_grid_wide.png"
           class="d-block w-100"
           alt="Research Figure 3">
    </div>
    <div class="carousel-item" data-caption="A comparison of the induced and Sasaki metrics, to appear in ICML">
      <img src="{{ site.baseurl }}/assets/images/sasaki.png"
           class="d-block w-100"
           alt="Research Figure 4">
    </div>
    <div class="carousel-item" data-caption="A comparison of Laplacian eigenfunctions between a clean and noisy manifold, to appear in ICML">
      <img src="{{ site.baseurl }}/assets/images/clean_vs_noisy.png"
           class="d-block w-100"
           alt="Research Figure 5">
    </div>
    <div class="carousel-item" data-caption="Neighborhoods produced by AGOP Descent, coming research">
      <img src="{{ site.baseurl }}/assets/images/Mandrill_Localizations_2.png"
           class="d-block w-100"
           alt="Research Figure 6">
    </div>
    <div class="carousel-item" data-caption="AGOP Descent performed on a toy dataset, coming research">
      <img src="{{ site.baseurl }}/assets/images/AGOP_descent-1.png"
           class="d-block w-100"
           alt="Research Figure 7">
    </div>
  </div>

  <!-- Navigation controls (previous/next arrows) -->
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

<!-- Caption initialization script -->
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
