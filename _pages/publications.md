---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 2
---

<style>
  /* Page heading */
  .post-header {
    margin-bottom: 1.2rem !important;
  }

  .post-header .post-title {
    margin: 0 !important;
    color: var(--global-text-color);
    font-size: 2.6rem !important;
    font-weight: 500;
    line-height: 1.15;
  }

  .post-header .post-description {
    display: none !important;
  }

  /* Year and publication list layout */
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
    margin: 0.7rem 0 0 !important;
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
    margin: 0.7rem 0 0 !important;
    padding-top: 1rem;
    padding-left: 0;
    border-top: 1px solid var(--global-divider-color);
  }

  .publications ol.bibliography > li {
    margin-bottom: 1.7rem !important;
  }

  /* Remove unnecessary indentation inside each entry */
  .publications ol.bibliography li .row {
    align-items: flex-start;
  }

  /* Journal abbreviation */
  .publications .abbr {
    padding-top: 0.15rem;
  }

  .publications .abbr abbr {
    border-radius: 0 !important;
    background-color: var(--global-theme-color) !important;
    color: #ffffff !important;
    font-size: 0.75rem;
    font-weight: 600;
  }

  /* Publication title */
  .publications .title {
    margin-bottom: 0.25rem !important;
    color: var(--global-text-color);
    font-size: 1.12rem !important;
    font-weight: 600 !important;
    line-height: 1.35;
  }

  /* Authors */
  .publications .author {
    margin-bottom: 0.2rem !important;
    color: var(--global-text-color);
    font-size: 0.94rem;
    line-height: 1.45;
  }

  /* Journal, volume, pages and year */
  .publications .periodical {
    display: inline;
    margin: 0 !important;
    color: var(--global-text-color-light);
    font-size: 0.9rem;
    line-height: 1.45;
  }

  .publications .periodical em {
    color: var(--global-text-color);
  }

  /* DOI and other links */
  .publications .links {
    display: inline;
    margin-left: 0.45rem;
    white-space: normal;
  }

  .publications .links a {
    display: inline-block;
    margin: 0 0.2rem 0.2rem 0 !important;
    padding: 0.16rem 0.48rem !important;
    border: 1px solid var(--global-divider-color) !important;
    border-radius: 0 !important;
    background-color: transparent !important;
    color: var(--global-text-color) !important;
    font-size: 0.7rem !important;
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

  /* Extra publication information */
  .publications .periodical + .additional-info,
  .publications .additional-info {
    margin-top: 0.3rem;
    color: var(--global-text-color-light);
    font-size: 0.86rem;
    line-height: 1.4;
  }

  /* Mobile layout */
  @media (max-width: 575px) {
    .post-header {
      margin-bottom: 0.8rem !important;
    }

    .post-header .post-title {
      font-size: 2rem !important;
    }

    .publications {
      grid-template-columns: 42px minmax(0, 1fr);
      column-gap: 0.65rem;
    }

    .publications h2.bibliography {
      font-size: 0.82rem !important;
    }

    .publications ol.bibliography > li {
      margin-bottom: 1.4rem !important;
    }

    .publications .title {
      font-size: 1rem !important;
    }

    .publications .author {
      font-size: 0.86rem;
    }

    .publications .periodical {
      font-size: 0.83rem;
    }

    .publications .abbr {
      display: none;
    }

    .publications ol.bibliography li .col-sm-8,
    .publications ol.bibliography li .col-sm-10 {
      width: 100%;
      max-width: 100%;
      padding-right: 0;
      padding-left: 0;
      flex: 0 0 100%;
    }
  }
</style>

<div class="publications">{% bibliography %}</div>
