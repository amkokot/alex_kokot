---
layout: main
title: "Home"
permalink: /index-test/
---

<div class="intro-inline">
  <img 
    src="{{ site.baseurl }}/assets/images/alex_kokot.jpg" 
    alt="Alex Kokot" 
    class="intro-img"
  />
  <div class="intro-text">
    <h2>Alex Kokot</h2>
    <p class="lead text-secondary">
      Ph.D. Candidate in Statistics at the University of Washington.
    </p>
    
    <p>
      In my research, I incorporate <strong>geometric principles</strong> into the analysis of functionals arising in statistics and machine learning. Key research themes include:
    </p>
    <ul>
      <li>Making ML algorithms more <strong>computationally</strong> and <strong>statistically efficient</strong>.</li>
      <li>Leveraging <strong>geometric structure</strong> in data.</li>
      <li>Re-imagining classical methods in <strong>modern settings</strong>.</li>
    </ul>
    <p>
      To tackle these problems, I use tools from <strong>functional analysis</strong>, <strong>entropic optimal transport</strong>, <strong>numerical linear algebra</strong>, and <strong>empirical processes</strong>.
    </p>

    <div class="mt-4 pt-3 border-top">
      <p class="small text-muted mb-2">
        <strong>Advisors:</strong> <a href="https://stat.uw.edu/about-us/people/marina-meila" class="text-decoration-none text-muted">Marina Meilã</a> & <a href="https://stat.uw.edu/about-us/people/alex-luedtke" class="text-decoration-none text-muted">Alex Luedtke</a><br>
        <strong>Defense:</strong> June 2026
      </p>
      <a href="{{ site.baseurl }}/research/" class="btn btn-primary btn-sm me-2">View Portfolio</a>
      <a href="{{ site.baseurl }}/assets/Documents/CV_Kokot.pdf" target="_blank" class="btn btn-outline-dark btn-sm">Download CV</a>
    </div>
  </div>
</div>

<hr class="my-5">

<h3 class="h5 text-muted mb-3">Visualizing Research</h3>

<div id="researchCarousel" class="carousel slide mb-4 shadow-sm border rounded" data-bs-ride="carousel">
  <div class="carousel-inner rounded">
    
    <div class="carousel-item active" data-caption="<strong>Coreset Selection:</strong> Treemap of a Sinkhorn coreset from MNIST data.">
      <img src="{{ site.baseurl }}/assets/images/mnist_treemap.png" class="d-block w-100" alt="MNIST Treemap">
    </div>

    <div class="carousel-item" data-caption="<strong>Entropic OT:</strong> Geometric visualization of a Sinkhorn coreset.">
      <img src="{{ site.baseurl }}/assets/images/mnist_scatter_categorical.png" class="d-block w-100" alt="MNIST Scatter">
    </div>

    <div class="carousel-item" data-caption="<strong>Distributional Compression:</strong> Sinkhorn coresets from a Gaussian mixture.">
      <img src="{{ site.baseurl }}/assets/images/gauss_grid_wide.png" class="d-block w-100" alt="Gaussian Grid">
    </div>

    <div class="carousel-item" data-caption="<strong>Spectral Embeddings:</strong> A comparison of the induced and Sasaki metrics. (To appear in ICML)">
      <img src="{{ site.baseurl }}/assets/images/sasaki.png" class="d-block w-100" alt="Sasaki Metric">
    </div>

    <div class="carousel-item" data-caption="<strong>Manifold Learning:</strong> Laplacian eigenfunctions on clean vs. noisy manifolds.">
      <img src="{{ site.baseurl }}/assets/images/clean_vs_noisy.png" class="d-block w-100" alt="Clean vs Noisy">
    </div>

    <div class="carousel-item" data-caption="<strong>Local EGOP:</strong> Neighborhoods produced by AGOP Descent.">
      <img src="{{ site.baseurl }}/assets/images/Mandrill_Localizations_2.png" class="d-block w-100" alt="Mandrill Localizations">
    </div>

  </div>

  <button class="carousel-control-prev" type="button" data-bs-target="#researchCarousel" data-bs-slide="prev">
    <span class="carousel-control-prev-icon bg-dark rounded-circle p-2" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#researchCarousel" data-bs-slide="next">
    <span class="carousel-control-next-icon bg-dark rounded-circle p-2" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>

<div class="text-center mt-2">
  <p id="carouselCaption" class="text-muted small"></p>
</div>

<script>
  document.addEventListener('DOMContentLoaded', function() {
    const carousel = document.getElementById('researchCarousel');
    const captionContainer = document.getElementById('carouselCaption');

    function updateCaption() {
      const activeItem = carousel.querySelector('.carousel-item.active');
      const captionHTML = activeItem.getAttribute('data-caption');
      captionContainer.innerHTML = captionHTML || '';
    }

    carousel.addEventListener('slid.bs.carousel', updateCaption);
    updateCaption();
  });
</script>