---
layout: page
title: Research
permalink: /research/
description:
nav: true
nav_order: 2
---

<style>
  .research-page,
  .research-page * {
    color: var(--global-text-color);
  }

  .research-intro {
    max-width: 920px;
    margin: 0 0 3.5rem;
    color: var(--global-text-color);
    font-size: 1.05rem;
    line-height: 1.75;
  }

  .research-section {
    display: grid;
    grid-template-columns: minmax(0, 1.35fr) minmax(280px, 0.65fr);
    gap: 3.5rem;
    align-items: center;
    padding: 3rem 0;
    border-top: 1px solid var(--global-divider-color);
  }

  .research-section:first-of-type {
    padding-top: 2.5rem;
  }

  .research-content {
    min-width: 0;
  }

  .research-number {
    margin: 0 0 0.45rem;
    color: var(--global-theme-color);
    font-size: 2.4rem;
    font-weight: 700;
    line-height: 1;
  }

  .research-stage {
    margin: 0 0 0.55rem;
    color: var(--global-text-color-light);
    font-size: 0.76rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    line-height: 1.4;
    text-transform: uppercase;
  }

  .research-title {
    margin: 0 0 1rem;
    color: var(--global-text-color);
    font-size: 1.65rem;
    font-weight: 700;
    line-height: 1.3;
  }

  .research-question {
    margin: 0 0 1.1rem;
    padding-left: 1rem;
    border-left: 3px solid var(--global-theme-color);
    color: var(--global-text-color);
    font-size: 1rem;
    font-style: italic;
    line-height: 1.6;
  }

  .research-description {
    margin: 0;
    color: var(--global-text-color);
    font-size: 0.95rem;
    line-height: 1.75;
  }

  .research-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-top: 1.4rem;
  }

  .research-tag {
    display: inline-block;
    padding: 0.3rem 0.65rem;
    border: 1px solid var(--global-divider-color);
    color: var(--global-text-color-light);
    font-size: 0.72rem;
    font-weight: 500;
    line-height: 1.3;
  }

  .research-figure {
    margin: 0;
  }

  .research-image {
    display: block;
    width: 100%;
    aspect-ratio: 4 / 3;
    border: 1px solid var(--global-divider-color);
    border-radius: 0;
    background-color: var(--global-card-bg-color);
    object-fit: cover;
  }

  .research-caption {
    margin-top: 0.65rem;
    color: var(--global-text-color-light);
    font-size: 0.72rem;
    line-height: 1.45;
  }

  .research-caption strong {
    color: var(--global-text-color);
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.06em;
  }

  @media (min-width: 768px) {
    .research-section:nth-of-type(even) .research-content {
      order: 2;
    }

    .research-section:nth-of-type(even) .research-figure {
      order: 1;
    }
  }

  @media (max-width: 767px) {
    .research-intro {
      margin-bottom: 2rem;
      font-size: 0.96rem;
    }

    .research-section {
      grid-template-columns: 1fr;
      gap: 1.7rem;
      padding: 2.3rem 0;
    }

    .research-number {
      font-size: 2rem;
    }

    .research-title {
      font-size: 1.35rem;
    }

    .research-question {
      font-size: 0.92rem;
    }

    .research-description {
      font-size: 0.9rem;
    }

    .research-figure {
      max-width: 520px;
    }
  }
</style>

<div class="research-page">
  <p class="research-intro">
    My research focuses on the design of
    <strong>functional and responsive coordination materials</strong>. I am
    particularly interested in understanding how molecular-level composition,
    structure, and dynamics translate into collective properties within
    crystalline solids.
  </p>

  <!-- RESEARCH 01 -->
  <section class="research-section">
    <div class="research-content">
      <div class="research-number">01</div>
      <div class="research-stage">PhD Research</div>

      <h2 class="research-title">
        Structural Control in Metal–Organic Frameworks
      </h2>

      <p class="research-question">
        How do MOF structures accommodate compositional and structural
        perturbations?
      </p>

      <p class="research-description">
        My PhD research focused on understanding and controlling structural
        changes in metal–organic frameworks (MOFs). I studied how framework
        structures respond to lattice mismatch, mixed-linker composition,
        defects, and guest adsorption. Through these studies, I became
        particularly interested in how small changes in molecular components can
        lead to significant changes in crystalline structures and their
        properties.
      </p>

      <div class="research-tags">
        <span class="research-tag">MOF-on-MOF Growth</span>
        <span class="research-tag">Lattice Mismatch</span>
        <span class="research-tag">Mixed-Linker Systems</span>
        <span class="research-tag">Defects</span>
        <span class="research-tag">Gate Opening</span>
      </div>
    </div>

    <figure class="research-figure">
      <img
        class="research-image"
        src="/assets/img/research-01.jpg"
        alt="Structural control in metal–organic frameworks"
      >
      <figcaption class="research-caption">
        <strong>RESEARCH IMAGE 01</strong><br>
        Representative structures from MOF-on-MOF, mixed-linker, defect, and
        gate-opening studies.
      </figcaption>
    </figure>
  </section>

  <!-- RESEARCH 02 -->
  <section class="research-section">
    <div class="research-content">
      <div class="research-number">02</div>
      <div class="research-stage">Postdoctoral Research</div>

      <h2 class="research-title">
        Stimulus-Responsive Coordination Materials
      </h2>

      <p class="research-question">
        Can a functional molecule retain its dynamic behavior when incorporated
        into a coordination solid?
      </p>

      <p class="research-description">
        My current postdoctoral research expands my interest from framework-level
        structural changes to molecular-level dynamics within coordination
        solids. I design and synthesize functional ligands that can change their
        molecular states in response to external stimuli and investigate whether
        these properties are retained after incorporation into crystalline
        coordination materials. This work combines ligand synthesis,
        coordination chemistry, structural characterization, and computational
        analysis.
      </p>

      <div class="research-tags">
        <span class="research-tag">Functional Ligands</span>
        <span class="research-tag">Photoswitching</span>
        <span class="research-tag">Coordination Solids</span>
        <span class="research-tag">Structural Characterization</span>
        <span class="research-tag">Computational Analysis</span>
      </div>
    </div>

    <figure class="research-figure">
      <img
        class="research-image"
        src="/assets/img/research-02.jpg"
        alt="Stimulus-responsive coordination materials"
      >
      <figcaption class="research-caption">
        <strong>RESEARCH IMAGE 02</strong><br>
        Functional ligand structures, stimulus-induced molecular changes, or a
        representative coordination-solid structure.
      </figcaption>
    </figure>
  </section>

  <!-- RESEARCH 03 -->
  <section class="research-section">
    <div class="research-content">
      <div class="research-number">03</div>
      <div class="research-stage">Independent Research Direction</div>

      <h2 class="research-title">Molecular-to-Solid Function</h2>

      <p class="research-question">
        What determines whether molecular function is preserved, suppressed, or
        transformed in a crystalline solid?
      </p>

      <p class="research-description">
        My future independent research will focus on understanding how molecular
        functions change when functional molecules are incorporated into
        crystalline solids. A molecule that works well in solution may retain,
        lose, or show a different function in the solid state because of
        coordination, molecular packing, and local environments. I aim to
        understand the structural factors that determine these differences and
        ultimately develop more predictable strategies for designing functional
        solid materials.
      </p>

      <div class="research-tags">
        <span class="research-tag">Molecular Function</span>
        <span class="research-tag">Solid-State Environment</span>
        <span class="research-tag">Molecular Packing</span>
        <span class="research-tag">Structure–Function Relationships</span>
        <span class="research-tag">Predictive Materials Design</span>
      </div>
    </div>

    <figure class="research-figure">
      <img
        class="research-image"
        src="/assets/img/research-03.jpg"
        alt="Molecular-to-solid function"
      >
      <figcaption class="research-caption">
        <strong>RESEARCH IMAGE 03</strong><br>
        A conceptual connection between molecular structure, coordination,
        packing, crystalline structure, and material function.
      </figcaption>
    </figure>
  </section>

  <!-- RESEARCH 04 -->
  <section class="research-section">
    <div class="research-content">
      <div class="research-number">04</div>
      <div class="research-stage">Collaborative Research Direction</div>

      <h2 class="research-title">
        Data-Driven Design of Functional Solids
      </h2>

      <p class="research-question">
        How can experimental structure–function data guide the prediction of
        functional crystalline materials?
      </p>

      <p class="research-description">
        I am also interested in developing data-driven approaches for the design
        of functional crystalline solids through collaborative research. By
        combining experimental structure–function data from my research with
        machine learning and deep learning, we aim to identify molecular and
        structural factors that determine the functions of crystalline
        materials. Ultimately, I hope this collaboration will help us screen
        promising molecular and solid-state candidates before synthesis and make
        the discovery of functional materials more efficient and predictable.
      </p>

      <div class="research-tags">
        <span class="research-tag">Experimental Data</span>
        <span class="research-tag">Machine Learning</span>
        <span class="research-tag">Deep Learning</span>
        <span class="research-tag">Descriptor Identification</span>
        <span class="research-tag">Candidate Prediction</span>
        <span class="research-tag">Experimental Validation</span>
      </div>
    </div>

    <figure class="research-figure">
      <img
        class="research-image"
        src="/assets/img/research-04.jpg"
        alt="Data-driven design of functional solids"
      >
      <figcaption class="research-caption">
        <strong>RESEARCH IMAGE 04</strong><br>
        Experimental structure–function data, computational prediction, and
        experimental validation of candidate materials.
      </figcaption>
    </figure>
  </section>
</div>
