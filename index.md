---
layout: main
title: "Home"
permalink: /
---


<!-- Carousel component (Bootstrap) -->
<div id="researchCarousel" class="carousel slide mb-4" data-bs-ride="carousel">
  <!-- Indicators (dots) if you want clickable slide indicators -->
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#researchCarousel" data-bs-slide-to="0" class="active"></button>
    <button type="button" data-bs-target="#researchCarousel" data-bs-slide-to="1"></button>
    <button type="button" data-bs-target="#researchCarousel" data-bs-slide-to="2"></button>
    <!-- Add more buttons if more slides -->
  </div>
  <!-- Slides -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="/assets/images/figure1.png" class="d-block w-100" alt="Research Figure 1">
      <div class="carousel-caption">
        <p>Caption for figure 1 (optional)</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="/assets/images/figure2.png" class="d-block w-100" alt="Research Figure 2">
      <div class="carousel-caption">
        <p>Caption for figure 2 (optional)</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="/assets/images/figure3.png" class="d-block w-100" alt="Research Figure 3">
      <div class="carousel-caption">
        <p>Caption for figure 3 (optional)</p>
      </div>
    </div>
    <!-- Add more .carousel-item blocks if you have more images -->
  </div>
  <!-- Navigation controls (previous/next arrows) -->
  <button class="carousel-control-prev" type="button" data-bs-target="#researchCarousel" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#researchCarousel" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
