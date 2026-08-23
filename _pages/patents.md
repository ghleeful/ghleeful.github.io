---
layout: page
permalink: /patents/
title: Patents
description:
nav: true
nav_order: 4
---

<style>
  /* Overall page width */
  .container[role="main"] {
    width: 86% !important;
    max-width: 1320px !important;
  }

  /* Page heading */
  .post-header {
    margin-bottom: 0.9rem !important;
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

  /* Patent list */
  .patent-list {
    margin-top: 0.45rem;
  }

  .patent-entry {
    display: grid;
    grid-template-columns: 58px minmax(0, 1fr);
    column-gap: 1.25rem;
    padding: 0.9rem 0 1.5rem;
    border-top: 1px solid var(--global-divider-color);
  }

  /* Year */
  .patent-year {
    color: var(--global-text-color);
    font-size: 0.92rem;
    font-weight: 600;
    line-height: 1.3;
  }

  /* Patent information */
  .patent-content {
    max-width: 1050px;
  }

  .patent-title {
    margin: 0 0 0.3rem;
    color: var(--global-text-color);
    font-size: 1.03rem;
    font-weight: 600;
    line-height: 1.4;
  }

  .patent-inventors {
    margin: 0 0 0.2rem;
    color: var(--global-text-color);
    font-size: 0.9rem;
    line-height: 1.45;
  }

  .patent-details {
    margin: 0;
    color: var(--global-text-color-light);
    font-size: 0.87rem;
    line-height: 1.45;
  }

  .patent-status {
    display: inline-block;
    margin-left: 0.35rem;
    padding: 0.12rem 0.4rem;
    border: 1px solid var(--global-divider-color);
    color: var(--global-text-color);
    font-size: 0.66rem;
    font-weight: 500;
    line-height: 1.2;
    vertical-align: middle;
  }

  /* Mobile layout */
  @media (max-width: 575px) {
    .container[role="main"] {
      width: 100% !important;
      max-width: 100% !important;
      padding-right: 1rem !important;
      padding-left: 1rem !important;
    }

    .post-header {
      margin-bottom: 0.6rem !important;
    }

    .post-header .post-title {
      font-size: 1.8rem !important;
    }

    .patent-entry {
      grid-template-columns: 38px minmax(0, 1fr);
      column-gap: 0.6rem;
      padding: 0.75rem 0 1.2rem;
    }

    .patent-year {
      font-size: 0.76rem;
    }

    .patent-title {
      font-size: 0.94rem;
    }

    .patent-inventors {
      font-size: 0.82rem;
    }

    .patent-details {
      font-size: 0.8rem;
    }

    .patent-status {
      margin-top: 0.2rem;
      margin-left: 0;
      font-size: 0.62rem;
    }
  }
</style>

<div class="patent-list">
  <article class="patent-entry">
    <div class="patent-year">2026</div>

    <div class="patent-content">
      <h2 class="patent-title">
        Drop-and-Drain Method for Convenient and Efficient Fabrication of
        MOF/Fiber Composites
      </h2>

      <p class="patent-inventors">
        Moonhyun Oh, Hyunjeong Oh, and <u>Gihyun Lee</u>
      </p>

      <p class="patent-details">
        Korean Patent Registration No. 10-2986030
        <span class="patent-status">Registered</span>
      </p>
    </div>
  </article>

  <article class="patent-entry">
    <div class="patent-year">2023</div>

    <div class="patent-content">
      <h2 class="patent-title">
        Drop-and-Drain Method for Convenient and Efficient Fabrication of
        MOF/Fiber Composites
      </h2>

      <p class="patent-inventors">
        Moonhyun Oh, Hyunjeong Oh, and <u>Gihyun Lee</u>
      </p>

      <p class="patent-details">
        Korean Patent Application No. 10-2023-0135860
        <span class="patent-status">Application</span>
      </p>
    </div>
  </article>
</div>
