---
layout: main
title: "Research"
permalink: /research-test/
---

<style>
  /* 1. The Animation: Lift up and shadow on hover */
  .hover-card {
    transition: transform 0.25s ease-out, box-shadow 0.25s ease-out;
    cursor: pointer; 
  }

  .hover-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.1) !important;
  }

  /* 2. Image sizing */
  .research-img {
    height: 200px; 
    object-fit: cover; 
    object-position: center;
    border-bottom: 1px solid #eaecef;
  }

  /* 3. BibTeX styling */
  .bibtex-code {
    font-size: 0.75rem;
    background-color: #f8f9fa;
    padding: 10px;
    border-radius: 4px;
    margin-top: 5px;
    border: 1px solid #e9ecef;
  }

  /* 4. Footer Links Layering */
  .card-footer-actions {
    position: relative; 
    z-index: 2; 
    pointer-events: auto;
  }
</style>

## Research Overview
<p class="mb-5">
  In my research, I incorporate <strong>geometric principles</strong> into the analysis of functionals arising in statistics and machine learning.
  I focus on making ML algorithms computationally efficient, leveraging geometric structure in data, and re-imagining classical methods in modern settings.
</p>

<div class="row row-cols-1 row-cols-md-2 g-4 mb-5">

  <div class="col">
    <div class="card h-100 shadow-sm border-0 hover-card">
      <img src="{{ site.baseurl }}/assets/images/Mandrill_Localizations_2.png" class="card-img-top research-img" alt="Local EGOP">
      <div class="card-body d-flex flex-column position-relative">
        <a href="#" data-bs-toggle="modal" data-bs-target="#modalEGOP" class="stretched-link text-decoration-none">
          <h5 class="card-title text-dark">Local EGOP Learning</h5>
        </a>
        <h6 class="card-subtitle mb-2 text-muted">Kokot et al. (2025)</h6>
        <p class="card-text small text-secondary">
          A geometric model for structured data via the supervised noisy manifold hypothesis. We show that deep networks achieve an anisotropic metrization that simple models cannot.
        </p>
        <div class="mt-auto card-footer-actions pt-3 border-top">
           <a href="{{ site.baseurl }}/assets/Documents/EGOP_flow_v2.pdf" target="_blank" class="btn btn-sm btn-outline-primary py-0" style="font-size: 0.8rem;">Preprint</a>
        </div>
      </div>
    </div>
  </div>

  <div class="col">
    <div class="card h-100 shadow-sm border-0 hover-card">
      <img src="{{ site.baseurl }}/assets/images/gauss_grid_wide.png" class="card-img-top research-img" alt="Coreset Selection">
      <div class="card-body d-flex flex-column position-relative">
        <a href="#" data-bs-toggle="modal" data-bs-target="#modalCoreset" class="stretched-link text-decoration-none">
          <h5 class="card-title text-dark">Coreset Selection</h5>
        </a>
        <h6 class="card-subtitle mb-2 text-muted">Kokot & Luedtke (2025)</h6>
        <p class="card-text small text-secondary">
          A framework for selecting coresets with respect to arbitrary losses, including the Sinkhorn divergence. Also covers targeted sampling for fine-tuning and batch selection.
        </p>
        <div class="mt-auto card-footer-actions pt-3 border-top">
           <a href="https://arxiv.org/pdf/2504.20194" target="_blank" class="btn btn-sm btn-outline-primary py-0" style="font-size: 0.8rem;">PDF</a>
        </div>
      </div>
    </div>
  </div>

  <div class="col">
    <div class="card h-100 shadow-sm border-0 hover-card">
      <img src="{{ site.baseurl }}/assets/images/mnist_scatter_categorical.png" class="card-img-top research-img" alt="Entropic OT">
      <div class="card-body d-flex flex-column position-relative">
        <a href="#" data-bs-toggle="modal" data-bs-target="#modalEOT" class="stretched-link text-decoration-none">
          <h5 class="card-title text-dark">Entropic Optimal Transport</h5>
        </a>
        <h6 class="card-subtitle mb-2 text-muted">Theory & Limits</h6>
        <p class="card-text small text-secondary">
          Refining the analysis of the Sinkhorn divergence via Hadamard differentiability and deriving limits for self-EOT, establishing connections to spectral clustering.
        </p>
        <div class="mt-auto card-footer-actions pt-3 border-top">
           <span class="badge bg-light text-dark border">In Preparation</span>
        </div>
      </div>
    </div>
  </div>

  <div class="col">
    <div class="card h-100 shadow-sm border-0 hover-card">
      <img src="{{ site.baseurl }}/assets/images/sasaki.png" class="card-img-top research-img" alt="Spectral Embeddings">
      <div class="card-body d-flex flex-column position-relative">
        <a href="#" data-bs-toggle="modal" data-bs-target="#modalSpectral" class="stretched-link text-decoration-none">
          <h5 class="card-title text-dark">Geometrically Structured Data</h5>
        </a>
        <h6 class="card-subtitle mb-2 text-muted">Kokot, Murad, & Meila (2025)</h6>
        <p class="card-text small text-secondary">
          Rigorous analysis of spectral embeddings on noisy manifolds. Using the Sasaki metric, we show these embeddings detect structure beyond strict dimensionality.
        </p>
        <div class="mt-auto card-footer-actions pt-3 border-top">
           <a href="{{ site.baseurl }}/assets/Documents/Noisy_Lap_v4.pdf" target="_blank" class="btn btn-sm btn-outline-primary py-0" style="font-size: 0.8rem;">Preprint</a>
        </div>
      </div>
    </div>
  </div>

</div>


<div class="modal fade" id="modalEGOP" tabindex="-1" aria-hidden="true">
  <div class="modal-dialog modal-lg modal-dialog-centered modal-dialog-scrollable">
    <div class="modal-content">
      <div class="modal-header border-0 pb-0">
        <h4 class="modal-title fw-bold">Local EGOP Learning</h4>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body pt-2">
        <p class="text-muted fst-italic mb-4">Kokot et al. (2025)</p>
        
        <p>It is commonly speculated that machine learning algorithms more effectively leverage <strong>structured data</strong> than their classical counterparts. I developed a geometric model for such structure via the <em>supervised noisy manifold hypothesis</em>, where covariates are concentrated about a low-dimensional manifold, and labels do not depend on orthogonal deviations.</p>
        
        <p>This is an instance of our newly introduced setting of <em>continuous-index learning</em>. I study this problem via <strong>kernel smoothing</strong> in an adaptive Mahalanobis metric. The objective is to induce anisotropy, reducing estimator variance by elongating along the normal space and pooling additional low bias data points.</p>
        
        <div class="p-3 bg-light rounded my-3 border-start border-4 border-primary">
          <strong>Key Insight:</strong> My approach is motivated by metrization by the <strong>expected gradient outerproduct (EGOP)</strong>. Experimentally, we demonstrate that <strong>deep neural networks</strong> achieve a similar metrization, while two-layer neural networks cannot, even in overparameterized regimes.
        </div>
      </div>
      <div class="modal-footer border-0">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
      </div>
    </div>
  </div>
</div>

<div class="modal fade" id="modalCoreset" tabindex="-1" aria-hidden="true">
  <div class="modal-dialog modal-lg modal-dialog-centered modal-dialog-scrollable">
    <div class="modal-content">
      <div class="modal-header border-0 pb-0">
        <h4 class="modal-title fw-bold">Coreset Selection & Targeted Sampling</h4>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body pt-2">
        <p class="text-muted fst-italic mb-4">Kokot & Luedtke (2025)</p>
        
        <p>In this work, I took on the task of <strong>distributional compression</strong>. We seek to construct a 'coreset' of <em>m</em> observations such that, relative to a specified divergence <em>D</em>, the coreset's deviation from the empirical is of the same order as the empirical's deviation from the truth. This presents a substantial generalization of typical clustering and coreset selection settings, as the loss <em>D</em> is arbitrary.</p>
        
        <p>I developed the <strong>Coresets of Order 2 (CO2)</strong> algorithm, which reduces the problem to minimizing a quadratic form under affine and sparsity constraints. By verifying <strong>Hadamard differentiability</strong> of the entropic potentials in the Gaussian RKHS, we showed that only poly-log(<em>n</em>) samples are required to approximate the population distribution up to negligible error.</p>

        <h6 class="mt-4">Targeted Sampling & Fine-Tuning</h6>
        <p>Beyond theoretical bounds, this framework allows for the selection of coresets to optimize arbitrary functionals, including <strong>empirical risk minimization</strong>. In ongoing research, these methods are applied to select data to accelerate model fitting, with applications ranging from identifying corpuses for <strong>fine-tuning</strong> to <strong>batch selection</strong> in SGD.</p>
      </div>
      <div class="modal-footer border-0">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
      </div>
    </div>
  </div>
</div>

<div class="modal fade" id="modalEOT" tabindex="-1" aria-hidden="true">
  <div class="modal-dialog modal-lg modal-dialog-centered modal-dialog-scrollable">
    <div class="modal-content">
      <div class="modal-header border-0 pb-0">
        <h4 class="modal-title fw-bold">Entropic Optimal Transport (EOT)</h4>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body pt-2">
        <p class="text-muted fst-italic mb-4">Ongoing Research</p>
        
        <p>In my analysis of the Sinkhorn divergence, I verified Hadamard differentiability via an inverse function theorem applied to the <strong>Schrödinger equations</strong>, refining earlier approaches in the field. In current research, we are building on this methodology, deriving limits for self-EOT (entropic transport from a distribution to itself) as the regularization approaches zero.</p>
        
        <div class="p-3 bg-light rounded my-3 border-start border-4 border-primary">
          <strong>Key Result:</strong> By reparameterizing this equation, I derived explicit first order approximations of an appropriate analogue to the entropic potentials. This shows an asymptotic correspondence between <strong>diffusion maps</strong> and the entropic self-transport coupling, relating our coreset selection algorithm for the Sinkhorn divergence directly to <strong>spectral clustering</strong>.
        </div>
      </div>
      <div class="modal-footer border-0">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
      </div>
    </div>
  </div>
</div>

<div class="modal fade" id="modalSpectral" tabindex="-1" aria-hidden="true">
  <div class="modal-dialog modal-lg modal-dialog-centered modal-dialog-scrollable">
    <div class="modal-content">
      <div class="modal-header border-0 pb-0">
        <h4 class="modal-title fw-bold">Geometrically Structured Data</h4>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body pt-2">
        <p class="text-muted fst-italic mb-4">Kokot, Murad, & Meila (2025)</p>

        <p>I analyzed <strong>Laplacian spectral embeddings</strong> for manifold data injected with high-dimensional noise. The traditional folklore is that low-dimensional spectral embeddings are insensitive to such contamination. To verify this rigorously, I developed a metric perturbation argument, comparing the induced tube geometry to the "flattened" <strong>Sasaki metric</strong>.</p>
        
        <p>The Sasaki metric presents a natural splitting of manifold and noise information, decomposing the Neumann Laplacian into an intrinsic component and a high frequency perturbation. By leveraging <strong>perturbation theory for unbounded operators</strong>, I showed that in the continuum, low frequency eigenfunctions are nearly invariant to deviations away from the manifold.</p>
        
        <p>Rather than a stability result, we take the dual point of view: Laplacian spectral embeddings <strong>detect fundamental data structure</strong>, with a dependence that is not strictly dimensional.</p>
      </div>
      <div class="modal-footer border-0">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
      </div>
    </div>
  </div>
</div>