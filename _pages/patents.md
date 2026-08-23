---
layout: page
permalink: /patents/
title: Patents
description:
nav: true
nav_order: 4
---

<style>
  /* Page width */
  .container[role="main"] {
    width: 86%;
    max-width: 1320px;
  }

  /* Page title */
  h1.post-title {
    margin-bottom: 2.2rem;
    font-size: 2.5rem !important;
    font-weight: 400;
    line-height: 1.15;
  }

  /* Patent entry: year | date | information */
  .patent-entry {
    display: grid;
    grid-template-columns: 100px 70px minmax(0, 1fr);
    column-gap: 1.5rem;
    align-items: start;
    padding: 1.3rem 0 1.55rem;
    border-top: 1px solid var(--global-divider-color);
  }

  /* Year */
  .patent-year {
    margin: 0;
    color: var(--global-text-color);
    font-size: 1.8rem;
    font-weight: 600;
    line-height: 1.2;
  }

  /* Filing or registration date */
  .patent-date {
    margin: 0;
    padding-top: 0.32rem;
    color: var(--global-text-color-light);
    font-size: 0.8rem;
    font-weight: 500;
    line-height: 1.4;
    white-space: nowrap;
  }

  /* Patent content */
  .patent-content {
    min-width: 0;
  }

  /* Patent title */
  .patent-title {
    margin: 0 0 0.32rem;
    color: var(--global-text-color);
    font-size: 1.12rem;
    font-weight: 700;
    line-height: 1.35;
  }

  /* Inventors */
  .patent-inventors {
    margin: 0 0 0.2rem;
    color: var(--global-text-color);
    font-size: 0.82rem;
    line-height: 1.4;
  }

  /* Patent number */
  .patent-details {
    margin: 0;
    color: var(--global-text-color-light);
    font-size: 0.78rem;
    line-height: 1.4;
  }

  /* Current author's name */
  .patent-inventors .current-author {
    color: var(--global-text-color);
    text-decoration: underline;
    text-decoration-thickness: 1px;
    text-underline-offset: 0.15rem;
  }

  /* Mobile layout */
  @media (max-width: 575px) {
    .container[role="main"] {
      width: calc(100% - 2rem);
    }

    h1.post-title {
      margin-bottom: 1.5rem;
      font-size: 2rem !important;
    }

    .patent-entry {
      display: grid;
      grid-template-columns: auto 1fr;
      column-gap: 0.8rem;
      padding: 1rem 0 1.2rem;
    }

    .patent-year {
      font-size: 1.4rem;
    }

    .patent-date {
      padding-top: 0.18rem;
      font-size: 0.74rem;
    }

    .patent-content {
      grid-column: 1 / -1;
      margin-top: 0.7rem;
    }

    .patent-title {
      font-size: 1.02rem;
    }

    .patent-inventors {
      font-size: 0.78rem;
    }

    .patent-details {
      font-size: 0.74rem;
    }
  }
</style>

<div class="patent-list">
  <article class="patent-entry">
    <p class="patent-year">2026</p>

    <!-- 실제 등록 월·일로 변경 -->
    <p class="patent-date">MM.DD</p>

    <div class="patent-content">
      <h2 class="patent-title">
        Drop-and-Drain Method for Convenient and Efficient Fabrication of MOF/Fiber Composites
      </h2>

      <p class="patent-inventors">
        Moonhyun Oh, Hyunjeong Oh, and
        <span class="current-author">Gihyun Lee</span>
      </p>

      <p class="patent-details">
        Korean Patent Registration No. 10-2986030
      </p>
    </div>
  </article>

  <article class="patent-entry">
    <p class="patent-year">2023</p>

    <!-- 실제 출원 월·일로 변경 -->
    <p class="patent-date">MM.DD</p>

    <div class="patent-content">
      <h2 class="patent-title">
        Drop-and-Drain Method for Convenient and Efficient Fabrication of MOF/Fiber Composites
      </h2>

      <p class="patent-inventors">
        Moonhyun Oh, Hyunjeong Oh, and
        <span class="current-author">Gihyun Lee</span>
      </p>

      <p class="patent-details">
        Korean Patent Application No. 10-2023-0135860
      </p>
    </div>
  </article>
</div>
