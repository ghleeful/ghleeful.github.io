---
layout: page
permalink: /research/
title: Research
description:
nav: true
nav_order: 2
---

<style>
  /* Page width */
  .container[role="main"] {
    width: 86%;
    max-width: 1320px;
  }

  /* Page title */
  h1.post-title {
    margin-bottom: 1.2rem;
    font-size: 2.5rem !important;
    font-weight: 400;
    line-height: 1.15;
  }

  /* Introductory statement */
  .research-intro {
    max-width: 960px;
    margin: 0 0 3rem;
    color: var(--global-text-color);
    font-size: 1.02rem;
    line-height: 1.7;
  }

  .research-intro strong {
    font-weight: 600;
  }

  /* Complete research section */
  .research-section {
    display: grid;
    grid-template-columns: 115px minmax(0, 1fr) 340px;
    column-gap: 2.2rem;
    align-items: start;
    padding: 2rem 0 2.3rem;
    border-top: 1px solid var(--global-divider-color);
  }

  /* Left-side number and career stage */
  .research-index {
    padding-top: 0.15rem;
  }

  .research-number {
    display: block;
    margin-bottom: 0.4rem;
    color: var(--global-theme-color);
    font-size: 1.5rem;
    font-weight: 600;
    line-height: 1;
  }

  .research-stage {
    display: block;
    color: var(--global-text-color-light);
    font-size: 0.72rem;
    font-weight: 600;
    line-height: 1.35;
    letter-spacing: 0.05em;
    text-transform: uppercase;
  }

  /* Research text */
  .research-content {
    min-width: 0;
  }

  .research-title {
    margin: 0 0 0.7rem;
    color: var(--global-text-color);
    font-size: 1.3rem;
    font-weight: 700;
    line-height: 1.3;
  }

  /* Central research question */
  .research-question {
    margin: 0 0 1rem;
    padding-left: 0.85rem;
    border-left: 3px solid var(--global-theme-color);
    color: var(--global-text-color);
    font-size: 0.92rem;
    font-style: italic;
    line-height: 1.5;
  }

  .research-description {
    margin: 0;
    color: var(--global-text-color);
    font-size: 0.88rem;
    line-height: 1.65;
  }

  /* Research keywords */
  .research-keywords {
    display: flex;
    flex-wrap: wrap;
    gap: 0.35rem;
    margin-top: 1.15rem;
  }

  .research-keyword {
    display: inline-block;
    padding: 0.2rem 0.48rem;
    border: 1px solid var(--global-divider-color);
    color: var(--global-text-color-light);
    font-size: 0.67rem;
    font-weight: 500;
    line-height: 1.2;
  }

  /* Image area */
  .research-media {
    width: 100%;
    min-height: 225px;
  }

  .research-image {
    display: block;
    width: 100%;
    height: 225px;
    border: 1px solid var(--global-divider-color);
    border-radius: 0;
    background-color: var(--global-card-bg-color);
    object-fit: contain;
  }

  /* Placeholder shown until an image is uploaded */
  .research-placeholder {
    display: flex;
    width: 100%;
    height: 225px;
    padding: 1.2rem;
    border: 1px solid var(--global-divider-color);
    background-color: var(--global-card-bg-color);
    color: var(--global-text-color-light);
    align-items: center;
    justify-content: center;
    font-size: 0.72rem;
    line-height: 1.5;
    text-align: center;
  }

  .research-placeholder strong {
    display: block;
    margin-bottom: 0.35rem;
    color: var(--global-theme-color);
    font-size: 0.78rem;
    letter-spacing: 0.04em;
  }

  .research-placeholder[hidden] {
    display: none !important;
  }

  /* Subtle emphasis for future direction */
  .research-section.future .research-title {
    color: var(--global-theme-color);
  }

  /* Tablet */
  @media (max-width: 991px) {
    .research-section {
      grid-template-columns: 90px minmax(0, 1fr);
    }

    .research-media {
      grid-column: 2;
      width: 100%;
      max-width: 520px;
      margin-top: 1.4rem;
    }
  }

  /* Mobile */
  @media (max-width: 575px) {
    .container[role="main"] {
      width: calc(100% - 2rem);
    }

    h1.post-title {
      font-size: 2rem !important;
    }

    .research-intro {
      margin-bottom: 2rem;
      font-size: 0.9rem;
      line-height: 1.6;
    }

    .research-section {
      display: block;
      padding: 1.5rem 0 1.8rem;
    }

    .research-index {
      margin-bottom: 0.8rem;
    }

    .research-number {
      display: inline-block;
      margin-right: 0.55rem;
      margin-bottom: 0;
      font-size: 1.25rem;
    }

    .research-stage {
      display: inline-block;
      font-size: 0.65rem;
    }

    .research-title {
      font-size: 1.12rem;
    }

    .research-question {
      font-size: 0.84rem;
    }

    .research-description {
      font-size: 0.82rem;
    }

    .research-media {
      width: 100%;
      max-width: none;
      margin-top: 1.2rem;
    }

    .research-image,
    .research-placeholder {
      height: 200px;
    }
  }
</style>

<div class="research-intro">
  My research focuses on the design of <strong>functional and responsive coordination materials</strong>. I am particularly interested in understanding how molecular-level composition, structure, and dynamics translate into collective properties within crystalline solids.
</div>

<section class="research-section">
  <div class="research-index">
    <span class="research-number">01</span>
    <span class="research-stage">PhD Research</span>
  </div>

  <div class="research-content">
    <h2 class="research-title">Structural Control in Metal–Organic Frameworks</h2>

    <p class="research-question">
      How do MOF structures accommodate compositional and structural perturbations?
    </p>

    <p class="research-description">
      My PhD research focused on understanding and controlling structural changes in metal–organic frameworks (MOFs). I studied how framework structures respond to lattice mismatch, mixed-linker composition, defects, and guest adsorption. Through these studies, I became particularly interested in how small changes in molecular components can lead to significant changes in crystalline structures and their properties.
    </p>

    <div class="research-keywords">
      <span class="research-keyword">MOF-on-MOF Growth</span>
      <span class="research-keyword">Lattice Mismatch</span>
      <span class="research-keyword">Mixed-Linker Systems</span>
      <span class="research-keyword">Defects</span>
      <span class="research-keyword">Gate Opening</span>
    </div>
  </div>

  <div class="research-media">
    <img
      class="research-image"
      src="{{ '/assets/img/research/research-01.jpg' | relative_url }}"
      alt="Structural control in metal–organic frameworks"
      onerror="this.hidden = true; this.nextElementSibling.hidden = false;"
    >
    <div class="research-placeholder" hidden>
      <div>
        <strong>RESEARCH IMAGE 01</strong>
        Suggested image: a collage of representative structural figures from MOF-on-MOF, mixed-linker, defect, and gate-opening studies.
      </div>
    </div>
  </div>
</section>

<section class="research-section">
  <div class="research-index">
    <span class="research-number">02</span>
    <span class="research-stage">Postdoctoral Research</span>
  </div>

  <div class="research-content">
    <h2 class="research-title">Stimulus-Responsive Coordination Materials</h2>

    <p class="research-question">
      Can a functional molecule retain its dynamic behavior when incorporated into a coordination solid?
    </p>

    <p class="research-description">
      My current postdoctoral research expands my interest from framework-level structural changes to molecular-level dynamics within coordination solids. I design and synthesize functional ligands that can change their molecular states in response to external stimuli and investigate whether these properties are retained after incorporation into crystalline coordination materials. This work combines ligand synthesis, coordination chemistry, structural characterization, and computational analysis.
    </p>

    <div class="research-keywords">
      <span class="research-keyword">Functional Ligands</span>
      <span class="research-keyword">Photoswitching</span>
      <span class="research-keyword">Coordination Solids</span>
      <span class="research-keyword">Structural Characterization</span>
      <span class="research-keyword">Computational Analysis</span>
    </div>
  </div>

  <div class="research-media">
    <img
      class="research-image"
      src="{{ '/assets/img/research/research-02.jpg' | relative_url }}"
      alt="Stimulus-responsive coordination materials"
      onerror="this.hidden = true; this.nextElementSibling.hidden = false;"
    >
    <div class="research-placeholder" hidden>
      <div>
        <strong>RESEARCH IMAGE 02</strong>
        Suggested image: ligand structures, stimulus-induced molecular changes, or a representative coordination-solid structure.
      </div>
    </div>
  </div>
</section>

<section class="research-section future">
  <div class="research-index">
    <span class="research-number">03</span>
    <span class="research-stage">Independent Direction</span>
  </div>

  <div class="research-content">
    <h2 class="research-title">Molecular-to-Solid Function</h2>

    <p class="research-question">
      What determines whether molecular function is preserved, suppressed, or transformed in a crystalline solid?
    </p>

    <p class="research-description">
      My future independent research will focus on understanding how molecular functions change when functional molecules are incorporated into crystalline solids. A molecule that works well in solution may retain, lose, or show a different function in the solid state because of coordination, molecular packing, and local environments. I aim to understand the structural factors that determine these differences and ultimately develop more predictable strategies for designing functional solid materials.
    </p>

    <div class="research-keywords">
      <span class="research-keyword">Molecular Function</span>
      <span class="research-keyword">Solid-State Environment</span>
      <span class="research-keyword">Molecular Packing</span>
      <span class="research-keyword">Structure–Function Relationships</span>
      <span class="research-keyword">Predictive Materials Design</span>
    </div>
  </div>

  <div class="research-media">
    <img
      class="research-image"
      src="{{ '/assets/img/research/research-03.jpg' | relative_url }}"
      alt="Molecular-to-solid function"
      onerror="this.hidden = true; this.nextElementSibling.hidden = false;"
    >
    <div class="research-placeholder" hidden>
      <div>
        <strong>RESEARCH IMAGE 03</strong>
        Suggested image: a conceptual diagram connecting molecule, coordination, packing, crystalline structure, and material function.
      </div>
    </div>
  </div>
</section>
<section class="research-item">
  <div class="research-number">04</div>

  <div class="research-content">
    <p class="research-stage">Collaborative Research Direction</p>

    <h2>Data-Driven Design of Functional Solids</h2>

    <p class="research-question">
      How can experimental structure–function data guide the prediction of
      functional crystalline materials?
    </p>

    <p>
      I am also interested in developing data-driven approaches for the design
      of functional crystalline solids through collaborative research. By
      combining experimental structure–function data from my research with
      machine learning and deep learning, we aim to identify molecular and
      structural factors that determine the functions of crystalline materials.
    </p>

    <p>
      Ultimately, I hope this collaboration will help us screen promising
      molecular and solid-state candidates before synthesis and make the
      discovery of functional materials more efficient and predictable.
    </p>

    <div class="research-workflow">
      <div>
        <strong>Experimental platform</strong>
        <span>
          Molecular and material design, synthesis, crystal structures, and
          structure–function measurements
        </span>
      </div>

      <div>
        <strong>Computational collaboration</strong>
        <span>
          Machine learning, deep learning, descriptor identification, and
          candidate prediction
        </span>
      </div>

      <div>
        <strong>Experimental validation</strong>
        <span>
          Synthesis and characterization of predicted molecular and solid-state
          candidates
        </span>
      </div>
    </div>
  </div>

  <div class="research-visual research-placeholder">
    <span>Research image</span>
    <small>data-driven-design.jpg</small>
  </div>
</section>
