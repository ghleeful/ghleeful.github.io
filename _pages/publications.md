---
layout: page
permalink: /publications/
title: Publications
description: Peer-reviewed publications in reverse chronological order.
nav: true
nav_order: 2
---

<style>
  /* Year on the left and publications on the right */
  .publications {
    display: grid;
    grid-template-columns: 75px minmax(0, 1fr);
    column-gap: 1.5rem;
    align-items: start;
  }

  /* Year */
  .publications h2.bibliography {
    position: static !important;
    grid-column: 1;
    width: auto !important;
    margin: 1.5rem 0 0 !important;
    padding-top: 1rem;
    border-top: 1px solid var(--global-divider-color);
    color: var(--global-text-color) !important;
    font-size: 1.05rem !important;
    font-weight: 600 !important;
    line-height: 1.2;
    text-align: left !important;
    opacity: 1 !important;
  }

  /* Publications belonging to each year */
  .publications ol.bibliography {
    grid-column: 2;
    margin: 1.5rem 0 0 !important;
    padding-top: 1rem;
    padding-left: 0;
    border-top: 1px solid var(--global-divider-color);
  }

  /* Individual publication */
  .publications ol.bibliography > li {
    margin-bottom: 1.75rem;
  }

  /* Mobile layout */
  @media (max-width: 575px) {
    .publications {
      grid-template-columns: 48px minmax(0, 1fr);
      column-gap: 0.75rem;
    }

    .publications h2.bibliography {
      font-size: 0.85rem !important;
    }

    .publications ol.bibliography > li {
      margin-bottom: 1.4rem;
    }
  }
</style>

<div class="publications">
  {% bibliography %}
</div>
