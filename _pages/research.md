---
layout: page
permalink: /research/
title: Research
description:
nav: true
nav_order: 2
---

<style>
  /* Overall page width */
  .container[role="main"] {
    width: 86% !important;
    max-width: 1320px !important;
  }

  /* Page heading */
  .post-header {
    margin-bottom: 1.1rem !important;
  }

  .post-header .post-title {
    margin: 0 !important;
    color: var(--global-text-color);
    font-size: 2.25rem !important;
    font-weight: 500 !important;
    line-height: 1.15;
  }

  .post-header .post-description {
    display: none !important;
  }

  /* Intro */
  .research-intro {
    max-width: 900px;
    margin-bottom: 2.4rem;
    color: var(--global-text-color);
    font-size: 1.05rem;
    line-height: 1.7;
  }

  .research-intro strong {
    color: var(--global-theme-color);
    font-weight: 600;
  }

  /* Research sections */
  .research-section {
    display: grid;
    grid-template-columns: minmax(0, 1.25fr) minmax(280px, 0.75fr);
    gap: 2.2rem;
    align-items: center;
    padding: 2rem 0;
    border-top: 1px solid var(--global-divider-color);
  }

  .research-section:nth-of-type(even) .research-text {
    order: 2;
  }

  .research-section:nth-of-type(even) .research-visual {
    order: 1;
  }

  .research-number {
    display: block;
    margin-bottom: 0.45rem;
    color: var(--global-theme-color);
    font-size: 0.76rem;
    font-weight: 600;
    letter-spacing: 0.12em;
  }

  .research-title {
    margin: 0 0 0.65rem;
    color: var(--global-text-color);
    font-size: 1.35rem;
    font-weight: 600;
    line-height: 1.35;
  }

  .research-text p {
    margin: 0;
    color: var(--global-text-color-light);
    font-size: 0.95rem;
    line-height: 1.65;
  }

  /* Image placeholders */
  .research-visual {
    display: flex;
    min-height: 220px;
    align-items: center;
    justify-content: center;
    border: 1px solid var(--global-divider-color);
    background:
      linear-gradient(
        135deg,
        rgba(140, 106, 36, 0.07),
        rgba(140, 106, 36, 0.015)
      );
    color: var(--global-text-color-light);
    text-align: center;
  }

  .research-placeholder span {
    display: block;
    margin-bottom: 0.3rem;
    color: var(--global-theme-color);
    font-size: 0.72rem;
    font-weight: 600;
    letter-spacing: 0.14em;
  }

  .research-placeholder small {
    font-size: 0.75rem;
  }

  /* Actual research images */
  .research-image {
    display: block;
    width: 100%;
    height: 250px;
    border-radius: 0;
    object-fit: cover;
  }

  /* Future direction */
  .research-future {
    margin-top: 0.5rem;
    padding: 2rem;
    border-top: 1px solid var(--global-divider-color);
    border-bottom: 1px solid var(--global-divider-color);
  }

  .research-future h2 {
    margin: 0 0 0.65rem;
    color: var(--global-text-color);
    font-size: 1.35rem;
    font-weight: 600;
  }

  .research-future p {
    max-width: 950px;
    margin: 0;
    color: var(--global-text-color-light);
    font-size: 0.95rem;
    line-height: 1.7;
  }

  /* Mobile */
  @media (max-width: 767px) {
    .container[role="main"] {
      width: 100% !important;
      max-width: 100% !important;
      padding-right: 1rem !important;
      padding-left: 1rem !important;
    }

    .post-header .post-title {
      font-size: 1.8rem !important;
    }

    .research-intro {
      margin-bottom: 1.6rem;
      font-size: 0.95rem;
    }

    .research-section {
      grid-template-columns: 1fr;
      gap: 1rem;
      padding: 1.5rem 0;
    }

    .research-section:nth-of-type(even) .research-text,
    .research-section:nth-of-type(even) .research-visual {
      order: initial;
    }

    .research-title {
      font-size: 1.15rem;
    }

    .research-text p {
      font-size: 0.88rem;
    }

    .research-visual {
      min-height: 180px;
    }

    .research-image {
      height: 210px;
    }

    .research-future {
      padding: 1.5rem 0;
    }
  }
</style>

<div class="research-intro">
  My research focuses on the design of
  <strong>functional and responsive coordination materials</strong>.
  I am particularly interested in understanding how molecular-level
  composition, structure, and dynamics translate into collective properties
  within crystalline solids.
</div>

<section class="research-section">
  <div class="research-text">
    <span class="research-number">RESEARCH 01</span>
    <h2 class="research-title">Responsive Porous Frameworks</h2>

    <p>
      I study structurally responsive metal–organic frameworks, including
      materials that undergo gate-opening behavior in response to guest
      adsorption. My goal is to understand the relationship between molecular
      structure, framework flexibility, and adsorption performance, and to use
      this understanding to improve the accessible capacity of porous
      materials.
    </p>
  </div>

  <div class="research-visual research-placeholder">
    <div>
      <span>IMAGE 01</span>
      <small>Gate-opening or adsorption figure</small>
    </div>
  </div>
</section>

<section class="research-section">
  <div class="research-text">
    <span class="research-number">RESEARCH 02</span>
    <h2 class="research-title">Multicomponent Frameworks</h2>

    <p>
      I explore how multiple metallic components can be positioned within
      metal–organic frameworks to create compositional and spatial complexity.
      This work includes programmable multimetallic arrangements and MOF-on-MOF
      growth, with an emphasis on controlling interactions between chemically
      distinct framework domains.
    </p>
  </div>

  <div class="research-visual research-placeholder">
    <div>
      <span>IMAGE 02</span>
      <small>Multimetallic MOF or MOF-on-MOF figure</small>
    </div>
  </div>
</section>

<section class="research-section">
  <div class="research-text">
    <span class="research-number">RESEARCH 03</span>
    <h2 class="research-title">Hybrid Materials and Processing</h2>

    <p>
      I am interested in integrating crystalline coordination materials with
      practical substrates and macroscopic structures. My previous work on
      MOF/fiber composites investigated convenient fabrication strategies for
      combining porous framework functionality with flexible fibrous
      materials.
    </p>
  </div>

  <div class="research-visual research-placeholder">
    <div>
      <span>IMAGE 03</span>
      <small>MOF/fiber composite or fabrication image</small>
    </div>
  </div>
</section>

<section class="research-future">
  <h2>Current and Future Directions</h2>

  <p>
    My continuing research aims to connect precise molecular and structural
    control with adaptive solid-state functions. I am interested in developing
    coordination materials whose responses can be programmed through
    composition, spatial organization, and framework dynamics, ultimately
    creating materials that actively respond to their chemical environment.
  </p>
</section>
