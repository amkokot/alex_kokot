---
layout: main
title: "Research"
permalink: /research/
---

<style>
  /* 1. Animation & Cursor */
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

  /* 4. Footer Links Layering (Fixes clickable buttons) */
  .card-footer-actions {
    position: relative; 
    z-index: 2; 
    pointer-events: auto;
  }
</style>

<div class="row mb-5">
  <div class="col-lg-8">
    <h2 class="mb-3">Research Overview</h2>
    <p class="text-secondary mb-3">
      For a comprehensive synthesis of my work and future research vision, please see my formal statement below.
    </p>
    <a href="{{ site.baseurl }}/assets/Documents/research_1_16.pdf" target="_blank" class="btn btn-outline-primary btn-sm">
      <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-file-earmark-pdf me-2" viewBox="0 0 16 16">
        <path d="M14 14V4.5L9.5 0H4a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h8a2 2 0 0 0 2-2zM9.5 3A1.5 1.5 0 0 0 11 4.5h2V14a1 1 0 0 1-1 1H4a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1h5.5v2z"/>
        <path d="M4.603 14.087a.81.81 0 0 1-.438-.42c-.195-.388-.13-.776.08-1.102.198-.307.526-.568.897-.787a7.68 7.68 0 0 1 1.482-.645 19.697 19.697 0 0 0 1.062-2.227 7.269 7.269 0 0 1-.43-1.295c-.086-.4-.119-.796-.046-1.136.075-.354.274-.672.65-.823.192-.077.4-.12.602-.077a.7.7 0 0 1 .477.365c.088.164.12.356.127.538.007.188-.012.396-.047.614-.084.51-.27 1.134-.52 1.794a10.954 10.954 0 0 0 .98 1.686 5.753 5.753 0 0 1 1.334.05c.364.066.734.195.96.465.12.144.193.32.2.518.007.192-.047.382-.138.563a1.04 1.04 0 0 1-.354.416.856.856 0 0 1-.51.138c-.331-.014-.654-.196-.933-.417a5.712 5.712 0 0 1-.911-.95 11.651 11.651 0 0 0-1.997.406 11.307 11.307 0 0 1-1.02 1.51c-.292.35-.609.656-.927.787a.793.793 0 0 1-.58.029zm1.379-1.901c-.166.076-.32.156-.459.238-.328.194-.541.383-.647.545-.094.145-.096.25-.04.361.01.022.02.036.026.044a.266.266 0 0 0 .035-.012c.137-.056.355-.235.635-.572a8.18 8.18 0 0 0 .45-.606zm1.64-1.33a12.71 12.71 0 0 1 1.01-.193 11.744 11.744 0 0 1-.51-.858 20.801 20.801 0 0 1-.5 1.05zm2.446.45c.15.163.296.3.435.41.24.19.407.253.498.256a.107.107 0 0 0 .07-.015.307.307 0 0 0 .094-.125.436.436 0 0 0 .059-.2.095.095 0 0 0-.026-.063c-.052-.062-.2-.152-.518-.209a3.876 3.876 0 0 0-.612-.053zM8.06 11.1c.15-.259.305-.528.466-.816a12.76 12.76 0 0 1-.922-.184.25.25 0 0 1-.006.004c-.004.01-.01.024-.015.04a2.95 2.95 0 0 0-.07.697zm1.144-8.818c-.024-.088-.046-.165-.062-.21a.502.502 0 0 0-.086-.115.088.088 0 0 0-.065-.035.088.088 0 0 0-.073.04.428.428 0 0 0-.045.16c-.012.067-.013.14-.002.213a.625.625 0 0 0 .034.167c.033.1.08.23.146.38.082.186.195.39.324.606.077-.282.164-.593.238-.894l-.509-.312z"/>
      </svg>
      Download Research Statement
    </a>
  </div>
</div>

<div class="row row-cols-1 row-cols-md-2 g-4 mb-5">

  <div class="col">
    <div class="card h-100 shadow-sm border-0 hover-card position-relative">
      <img src="{{ site.baseurl }}/assets/images/Mandrill_Localizations_2.png" class="card-img-top research-img" alt="Local EGOP">
      <div class="card-body d-flex flex-column">
        
        <a href="#" data-bs-toggle="modal" data-bs-target="#modalEGOP" class="stretched-link text-decoration-none">
          <h5 class="card-title text-dark">Local EGOP Learning</h5>
        </a>
        
        <h6 class="card-subtitle mb-2 text-muted">Kokot et al. (2025) · <span class="text-primary">Submitted to ICML</span></h6>
        
        <p class="card-text small text-secondary">
          A geometric model for structured data via the supervised noisy manifold hypothesis. We develop a method to capture the adaptivity deep networks achieve when the target function exhibits local low-dimensionaltity.
        </p>
        
        <div class="mt-auto card-footer-actions pt-3 border-top">
           <a href="https://arxiv.org/pdf/2601.07061" target="_blank" class="btn btn-sm btn-outline-primary py-0" style="font-size: 0.8rem;">PDF</a>
        </div>
      </div>
    </div>
  </div>

  <div class="col">
    <div class="card h-100 shadow-sm border-0 hover-card position-relative">
      <img src="{{ site.baseurl }}/assets/images/gauss_grid_wide.png" class="card-img-top research-img" alt="Coreset Selection">
      <div class="card-body d-flex flex-column">
        
        <a href="#" data-bs-toggle="modal" data-bs-target="#modalCoreset" class="stretched-link text-decoration-none">
          <h5 class="card-title text-dark">Coreset Selection</h5>
        </a>
        
        <h6 class="card-subtitle mb-2 text-muted">Kokot & Luedtke (2025) · <span class="text-primary">Submitted to JMLR</span></h6>
        
        <p class="card-text small text-secondary">
          A framework for selecting coresets with respect to arbitrary losses, including the Sinkhorn divergence.
        </p>
        
        <div class="mt-auto card-footer-actions pt-3 border-top">
           <a href="https://arxiv.org/pdf/2504.20194" target="_blank" class="btn btn-sm btn-outline-primary py-0" style="font-size: 0.8rem;">PDF</a>
        </div>
      </div>
    </div>
  </div>

  <div class="col">
    <div class="card h-100 shadow-sm border-0 hover-card position-relative">
      <img src="{{ site.baseurl }}/assets/images/astronaut_coreset.png" class="card-img-top research-img" alt="Entropic OT">
      <div class="card-body d-flex flex-column">
        
        <a href="#" data-bs-toggle="modal" data-bs-target="#modalEOT" class="stretched-link text-decoration-none">
          <h5 class="card-title text-dark">Entropic Optimal Transport</h5>
        </a>
        
        <h6 class="card-subtitle mb-2 text-muted">Kokot · <span class="text-warning text-dark">To be Submitted to SIMODS</span></h6>
        
        <p class="card-text small text-secondary">
          Refining the analysis of the Sinkhorn divergence via Hadamard differentiability and deriving limits for self-EOT, establishing connections to classical estimators in density and score estimation.
        </p>
        
        <div class="mt-auto card-footer-actions pt-3 border-top">
           <span class="badge bg-light text-dark border">Coming Soon</span>
        </div>
      </div>
    </div>
  </div>

  <div class="col">
    <div class="card h-100 shadow-sm border-0 hover-card position-relative">
      <img src="{{ site.baseurl }}/assets/images/sasaki.png" class="card-img-top research-img" alt="Spectral Embeddings">
      <div class="card-body d-flex flex-column">
        
        <a href="#" data-bs-toggle="modal" data-bs-target="#modalSpectral" class="stretched-link text-decoration-none">
          <h5 class="card-title text-dark">Geometrically Structured Data</h5>
        </a>
        
        <h6 class="card-subtitle mb-2 text-muted">Kokot, Murad, & Meila (2025) · <span class="text-success">ICML 2025</span></h6>
        
        <p class="card-text small text-secondary">
          Rigorous analysis of spectral embeddings on noisy manifolds. Using the Sasaki metric, we show these embeddings detect structure beyond strict dimensionality.
        </p>
        
        <div class="mt-auto card-footer-actions pt-3 border-top">
           <a href="{{ site.baseurl }}/assets/Documents/Noisy_Lap_v4.pdf" target="_blank" class="btn btn-sm btn-outline-primary py-0" style="font-size: 0.8rem;">PDF</a>
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
        
        <p>It is commonly speculated that machine learning algorithms more effectively leverage <strong>structured data</strong> than their classical counterparts. The <em>supervised noisy manifold hypothesis</em> is designed to capture this, with covariates concentrated about a low-dimensional manifold, and labels invariant to orthogonal deviations.</p>
        
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
        
        <p>We seek to construct a 'coreset' of <em>m</em> observations such that, relative to a specified divergence <em>D</em>, the coreset's deviation from the empirical is of the same order as the empirical's deviation from the truth. This presents a substantial generalization of typical clustering and coreset selection settings, as the loss <em>D</em> is arbitrary.</p>
        
        <p>I developed the <strong>Coresets of Order 2 (CO2)</strong> algorithm, which reduces the problem to minimizing a quadratic form under affine and sparsity constraints. By verifying <strong>Hadamard differentiability</strong> of the entropic potentials in the Gaussian RKHS, we showed that only poly-log(<em>n</em>) samples are required to approximate the population distribution up to negligible error.</p>

        <h6 class="mt-4">Targeted Sampling & Fine-Tuning</h6>
        <p>Beyond theoretical bounds, this framework allows for the selection of coresets to optimize arbitrary functionals, and this includes key settings such as <strong>empirical risk minimization</strong>. In ongoing research, these methods are applied to select data to accelerate model fitting, with applications ranging from identifying corpuses for <strong>fine-tuning</strong> to <strong>batch selection</strong> in SGD.</p>
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

        <p>We study <strong>Laplacian spectral embeddings</strong> for manifold data injected with high-dimensional noise. The traditional folklore is that low-dimensional spectral embeddings are insensitive to such contamination. To verify this rigorously, I developed a metric perturbation argument, comparing the induced tube geometry to the "flattened" <strong>Sasaki metric</strong>.</p>
        
        <p>The Sasaki metric presents a natural splitting of manifold and noise information, decomposing the Neumann Laplacian into an intrinsic component and a high frequency perturbation. By leveraging <strong>perturbation theory for unbounded operators</strong>, I showed that in the continuum, low frequency eigenfunctions are nearly invariant to deviations away from the manifold.</p>
        
        <p>Rather than a stability result, we take the dual point of view: Laplacian spectral embeddings <strong>detect fundamental data structure</strong>, with a dependence that is not strictly dimensional.</p>
      </div>
      <div class="modal-footer border-0">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
      </div>
    </div>
  </div>
</div>

<div class="mt-5 pt-4 border-top">
  <h2 class="h4 mb-4">Full Publication List</h2>

  <h3 class="h5 mt-4 mb-3 text-secondary border-bottom pb-2">In Preparation</h3>
  <ul class="list-unstyled">
    <li class="mb-3">
      <strong>Alex Kokot</strong>, Alex Luedtke, Marina Meila (2026).
      <em>Diffusion Maps are Entropic Self-Transport: Limits and Applications as ε→0</em>.
      To be submitted to <em>SIMODS</em>.
    </li>
  </ul>

  <h3 class="h5 mt-5 mb-3 text-secondary border-bottom pb-2">Submitted</h3>
  <ul class="list-unstyled">
    <li class="mb-3">
      Vydhourie Thiyageswaran, <strong>Alex Kokot</strong>, et al. (2026).
      <em>Optimal Design under Interference, Homophily, and Robustness Trade-offs</em>.
      Submitted to <em>JASA</em>.
    </li>
    <li class="mb-3">
       <strong>Alex Kokot</strong>, et al. (2026).
       <a href="https://arxiv.org/abs/2601.07061" target="_blank"><em>Local EGOP for Continuous Index Learning</em></a>.
       arXiv:2601.07061. Submitted to <em>ICML</em>.
    </li>
    <li class="mb-3">
      <strong>Alex Kokot</strong>, Alex Luedtke (2025).
      <a href="https://arxiv.org/abs/2504.20194" target="_blank"><em>Coreset selection for the Sinkhorn divergence and generic smooth divergences</em></a>.
      arXiv:2504.20194. Submitted to <em>JMLR</em> (under review).
    </li>
  </ul>

  <h3 class="h5 mt-5 mb-3 text-secondary border-bottom pb-2">Peer-Reviewed</h3>
  <ul class="list-unstyled">
    <li class="mb-3">
      <strong>Alex Kokot</strong>, Octavian-Vlad Murad, Marina Meila (2025).
      <a href="https://openreview.net/forum?id=GK6q2SFNHm" target="_blank"><em>The Noisy Laplacian: A threshold phenomenon for non-linear dimension reduction</em></a>.
      In <em>Proc. 42nd Int’l Conf. on Machine Learning (ICML 2025)</em>.
    </li>
    <li class="mb-3">
      Jose Agudelo, Brooke Dippold, Ian Klein, <strong>Alex Kokot</strong>, Eric Geiger, Irina Kogan (2024).
      <a href="https://msp.org/involve/2024/17-1/p03.xhtml" target="_blank"><em>Euclidean and affine curve reconstruction</em></a>.
      <em>Involve, a Journal of Mathematics</em>.
    </li>
    <li class="mb-3">
      Lei Zhang, Yu Wang, Mengyu Xu, <strong>Alex M. Kokot</strong>, Jie Qiu, Peter C. Burns (2024).
      <a href="https://doi.org/10.1039/D4CE00121D" target="_blank"><em>Hydrothermal synthesis and structure of organically templated layered neptunyl(VI) phosphate (NpO<sub>2</sub>)<sub>3</sub>(PO<sub>4</sub>)<sub>2</sub>(Terpy)</em></a>.
      <em>CrystEngComm</em>.
    </li>
    <li class="mb-3">
      Hrafn Traustason, Nicola L. Bell, Kiana Caranto, David C. Auld, David T. Lockey, <strong>Alex M. Kokot</strong>, Jennifer E. S. Szymanowski, Leroy Cronin, Peter C. Burns (2020).
      <a href="https://doi.org/10.1021/jacs.0c10133" target="_blank"><em>Reactivity, Formation, and Solubility of Polyoxometalates Probed by Calorimetry</em></a>.
      <em>Journal of the American Chemical Society</em>.
    </li>
    <li class="mb-3">
      Lei Zhang, Sergey M. Aksenov, <strong>Alex Kokot</strong>, Samuel N. Perry, Travis A. Olds, Peter C. Burns (2020).
      <a href="https://doi.org/10.1021/acs.inorgchem.0c00385" target="_blank"><em>Crystal Chemistry and Structural Complexity of Uranium(IV) Sulfates</em></a>.
      <em>Inorganic Chemistry</em>.
    </li>
    <li class="mb-3">
      Kulick, J., Nichols, B., Knight, T., Lu, T., Ortega, C., Siders, S., <strong>Kokot, A.</strong>, Bernstein, G. (2019).
      <a href="https://doi.org/10.1117/12.2518652" target="_blank"><em>Enabling curved hemispherical arrays with Quilt Packaging interconnect technology</em></a>.
      In <em>Proc. SPIE 10980</em>.
    </li>
    <li class="mb-3">
      Jie Qiu, Tyler L. Spano, Mateusz Dembowski, <strong>Alex Kokot</strong>, Jakub E. S. Szymanowski, Peter C. Burns (2017).
      <a href="https://doi.org/10.1021/acs.inorgchem.6b02429" target="_blank"><em>Sulfate-Centered Sodium-Icosahedron-Templated Uranyl Peroxide Phosphate Cages</em></a>.
      <em>Inorganic Chemistry</em>.
    </li>
  </ul>
</div>