---
layout: page
permalink: /publications/
title: Publications
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

  /* Year and publication layout */
  .publications {
    display: grid;
    grid-template-columns: 58px minmax(0, 1fr);
    column-gap: 1.25rem;
    width: 100%;
    align-items: start;
  }

  /* Year */
  .publications h2.bibliography {
    position: static !important;
    grid-column: 1;
    width: auto !important;
    margin: 0.45rem 0 0 !important;
    padding-top: 0.85rem;
    border-top: 1px solid var(--global-divider-color);
    color: var(--global-text-color) !important;
    font-size: 0.92rem !important;
    font-weight: 600 !important;
    line-height: 1.2;
    text-align: left !important;
    opacity: 1 !important;
  }

  /* Publication list for each year */
  .publications ol.bibliography {
    grid-column: 2;
    width: 100%;
    margin: 0.45rem 0 0 !important;
    padding-top: 0.85rem;
    padding-left: 0;
    border-top: 1px solid var(--global-divider-color);
  }

  .publications ol.bibliography > li {
    width: 100%;
    margin-bottom: 1.45rem !important;
  }

  .publications ol.bibliography li .row {
    width: 100%;
    margin-right: 0;
    margin-left: 0;
    align-items: flex-start;
  }

  /* Hide journal abbreviation badges */
  body .publications ol.bibliography li .row > .abbr,
  body .publications .abbr {
    display: none !important;
  }

  /* Allow publication information to use the available width */
  body .publications ol.bibliography li .row > .col-sm-8,
  body .publications ol.bibliography li .row > .col-sm-10 {
    width: 100% !important;
    max-width: 100% !important;
    padding-right: 0 !important;
    padding-left: 0 !important;
    flex: 0 0 100% !important;
  }

  /* Publication title */
  .publications .title {
    max-width: 1050px;
    margin-bottom: 0.22rem !important;
    color: var(--global-text-color);
    font-size: 1.03rem !important;
    font-weight: 600 !important;
    line-height: 1.35;
  }

  /* Authors */
  .publications .author {
    max-width: 1050px;
    margin-bottom: 0.15rem !important;
    color: var(--global-text-color);
    font-size: 0.9rem;
    line-height: 1.4;
  }

  /* Journal, volume, pages and year */
  .publications .periodical {
    display: inline;
    margin: 0 !important;
    color: var(--global-text-color-light);
    font-size: 0.87rem;
    line-height: 1.4;
  }

  .publications .periodical em {
    color: var(--global-text-color);
    font-weight: 400;
  }

  /* DOI link */
  .publications .links {
    display: inline;
    margin-left: 0.35rem;
    white-space: normal;
  }

  .publications .links a {
    display: inline-block;
    margin: 0 0.15rem 0.15rem 0 !important;
    padding: 0.12rem 0.4rem !important;
    border: 1px solid var(--global-divider-color) !important;
    border-radius: 0 !important;
    background-color: transparent !important;
    color: var(--global-text-color) !important;
    font-size: 0.66rem !important;
    font-weight: 500;
    line-height: 1.2;
    text-decoration: none;
    vertical-align: middle;
  }

  .publications .links a:hover {
    border-color: var(--global-theme-color) !important;
    background-color: var(--global-theme-color) !important;
    color: #ffffff !important;
  }

  /* Additional publication information */
  .publications .additional-info {
    margin-top: 0.25rem;
    color: var(--global-text-color-light);
    font-size: 0.82rem;
    line-height: 1.4;
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

    .publications {
      grid-template-columns: 38px minmax(0, 1fr);
      column-gap: 0.6rem;
    }

    .publications h2.bibliography {
      margin-top: 0.3rem !important;
      padding-top: 0.7rem;
      font-size: 0.76rem !important;
    }

    .publications ol.bibliography {
      margin-top: 0.3rem !important;
      padding-top: 0.7rem;
    }

    .publications ol.bibliography > li {
      margin-bottom: 1.25rem !important;
    }

    .publications .title {
      font-size: 0.94rem !important;
      line-height: 1.35;
    }

    .publications .author {
      font-size: 0.82rem;
    }

    .publications .periodical {
      font-size: 0.8rem;
    }

    .publications .links {
      margin-left: 0.2rem;
    }

    .publications .links a {
      padding: 0.1rem 0.35rem !important;
      font-size: 0.62rem !important;
    }
  }
</style>

<div class="publications">{% bibliography %}</div>
