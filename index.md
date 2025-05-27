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
      I’m a PhD student in the Department of Statistics at the University of Washington, advised by Marina Meila and Alex Luedtke. My main research interest is in data summarization. A conrete example of this is selecting representative subsamples from a dataset. One framing of this is coreset selection and clustering, where samples are chosen to minimize a loss of interest. Another is treatment assignment,
      where randomized designs are selected to minimize losses associated to certain potential outcome
      models and parameters of interest. I am lucky to have collaborated with a great team on this latter problem, with research soon to be released. One aim of my current research is to extend techniques from problems such as these to more general learning tasks, such as choosing good datasets to train ML models.

      As a dual question, I am also interested in the problem of "what summarizations are appropriate for certain datasets?" A primary example of this is dimension reduction. In recent work, we showed how spectral embeddings on manifolds with noise relate to their noiseless counterparts, and the extent of geometry recoverable in this setting. In current work we argue that the incorporation of supervised information allows for complete recovery, with techniques inspired by recent developments with the expected gradient outerproduct (EGOP).

      I have additionally considered problems regarding graph permanent estimation, comparing rankings, and many other settings which have caught my interest, particularly as they relate to the above perspectives. I am always looking for collaborators, please reach out if interested!
    </p>
  </div>
</div>

<!-- Carousel component (Bootstrap) -->
<div id="researchCarousel" class="carousel slide mb-4" data-bs-ride="carousel">
  <!-- Slides -->
  <div class="carousel-inner">
    <div class="carousel-item active" data-caption="Treemap of a Sinkhorn coreset from MNIST data https://arxiv.org/abs/2504.20194">
      <img src="{{ site.baseurl }}/assets/images/mnist_treemap.png"
           class="d-block w-100"
           alt="Research Figure 1">
    </div>
    <div class="carousel-item" data-caption="Geometric visualization of a Sinkhorn coreset from MNIST data https://arxiv.org/abs/2504.20194">
      <img src="{{ site.baseurl }}/assets/images/mnist_scatter_categorical.png"
           class="d-block w-100"
           alt="Research Figure 2">
    </div>
    <div class="carousel-item" data-caption="Sinkhorn coresets from a Gaussian mixture https://arxiv.org/abs/2504.20194">
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
