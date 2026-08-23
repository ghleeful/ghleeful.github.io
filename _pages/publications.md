---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 3
---

<style>
  /* Overall page width */
  .container[role="main"] {
    width: 86% !important;
    max-width: 1320px !important;
  }

  /* Page heading */
  .post-header {
    margin-bottom: 1rem !important;
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
    grid-template-columns: 90px minmax(0, 1fr);
    column-gap: 1.5rem;
    width: 100%;
    align-items: start;
  }

  /* Year */
  .publications h2.bibliography {
    position: static !important;
    grid-column: 1;
    width: auto !important;
    margin: 0.45rem 0 0 !important;
    padding-top: 1rem;
    border-top: 1px solid var(--global-divider-color);
    color: var(--global-text-color) !important;
    font-size: 1.8rem !important;
    font-weight: 600 !important;
    line-height: 1.1;
    text-align: left !important;
    opacity: 1 !important;
  }

  /* Publication list for each year */
  .publications ol.bibliography {
    grid-column: 2;
    width: 100%;
    margin: 0.45rem 0 0 !important;
    padding-top: 1rem;
    padding-left: 0;
    border-top: 1px solid var(--global-divider-color);
  }

  .publications ol.bibliography > li {
    width: 100%;
    margin-bottom: 1.8rem !important;
  }

  /* Each publication row */
  .publications ol.bibliography li .row {
    display: grid !important;
    grid-template-columns: minmax(0, 1fr);
    gap: 1.3rem;
    width: 100%;
    margin-right: 0;
    margin-left: 0;
    align-items: start;
  }

  /* Two-column layout only when a preview image exists */
  .publications ol.bibliography li .row:has(.abbr img.preview) {
    grid-template-columns: minmax(0, 1fr) 135px;
  }

  /* Publication text */
  body .publications ol.bibliography li .row > .col-sm-8,
  body .publications ol.bibliography li .row > .col-sm-10 {
    grid-column: 1;
    grid-row: 1;
    width: 100% !important;
    max-width: 100% !important;
    padding-right: 0 !important;
    padding-left: 0 !important;
    flex: 0 0 100% !important;
  }

  /* Hide abbreviation area when there is no image */
  body .publications .abbr:not(:has(img.preview)) {
    display: none !important;
  }

  /* Preview image area */
  body .publications .abbr:has(img.preview) {
    display: block !important;
    grid-column: 2;
    grid-row: 1;
    width: 135px !important;
    max-width: 135px !important;
    margin: 0 !important;
    padding: 0 !important;
  }

  /* Hide journal abbreviation badges */
  body .publications .abbr .badge {
    display: none !important;
  }

  /* Publication preview image */
  .publications .abbr img.preview {
    display: block;
    width: 135px !important;
    height: 135px !important;
    margin: 0 !important;
    border: 1px solid var(--global-divider-color);
    border-radius: 0 !important;
    background-color: #ffffff;
    box-shadow: none !important;
    object-fit: contain;
  }

  /* Publication title */
  .publications .title {
    max-width: 1050px;
    margin-bottom: 0.28rem !important;
    color: var(--global-text-color);
    font-size: 1.05rem !important;
    font-weight: 600 !important;
    line-height: 1.38;
  }

  /* Authors */
  .publications .author {
    max-width: 1050px;
    margin-bottom: 0.18rem !important;
    color: var(--global-text-color);
    font-size: 0.9rem;
    line-height: 1.45;
  }

  /* Journal, volume and pages */
  .publications .periodical {
    display: inline;
    margin: 0 !important;
    color: var(--global-text-color-light);
    font-size: 0.87rem;
    line-height: 1.45;
  }

  .publications .periodical em {
    color: var(--global-text-color);
    font-weight: 400;
  }

  /* DOI link */
  .publications .links {
    display: inline;
    margin-left: 0.4rem;
    white-space: normal;
  }

  .publications .links a {
    display: inline-block;
    margin: 0 0.15rem 0.15rem 0 !important;
    padding: 0.12rem 0.42rem !important;
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

  /* Tablet */
  @media (max-width: 900px) {
    .publications {
      grid-template-columns: 70px minmax(0, 1fr);
      column-gap: 1rem;
    }

    .publications h2.bibliography {
      font-size: 1.45rem !important;
    }

    .publications ol.bibliography li .row:has(.abbr img.preview) {
      grid-template-columns: minmax(0, 1fr) 110px;
    }

    body .publications .abbr:has(img.preview) {
      width: 110px !important;
      max-width: 110px !important;
    }

    .publications .abbr img.preview {
      width: 110px !important;
      height: 110px !important;
    }
  }

  /* Mobile */
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
      display: block;
    }

    .publications h2.bibliography {
      margin: 1.2rem 0 0 !important;
      padding-top: 0.75rem;
      font-size: 1.25rem !important;
    }

    .publications ol.bibliography {
      width: 100%;
      margin: 0 !important;
      padding-top: 0.7rem;
      border-top: 0;
    }

    .publications ol.bibliography > li {
      margin-bottom: 1.6rem !important;
    }

    .publications ol.bibliography li .row,
    .publications ol.bibliography li .row:has(.abbr img.preview) {
      display: flex !important;
      flex-direction: column;
      gap: 0.75rem;
    }

    body .publications ol.bibliography li .row > .col-sm-8,
    body .publications ol.bibliography li .row > .col-sm-10 {
      order: 1;
    }

    body .publications .abbr:has(img.preview) {
      order: 2;
      width: 100% !important;
      max-width: 100% !important;
    }

    .publications .abbr img.preview {
      width: 100% !important;
      max-width: 260px !important;
      height: auto !important;
      max-height: 230px;
      object-fit: contain;
    }

    .publications .title {
      font-size: 0.96rem !important;
      line-height: 1.4;
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

{% bibliography %}

<script>
  document.addEventListener("DOMContentLoaded", function () {
    const yearHeadings = document.querySelectorAll(
      ".publications h2.bibliography",
    );

    yearHeadings.forEach(function (heading) {
      const year = heading.textContent.trim();
      const publicationList = heading.nextElementSibling;

      if (!publicationList || !year) {
        return;
      }

      publicationList.querySelectorAll(".periodical").forEach(function (item) {
        const yearPattern = new RegExp(
          "\\s*,?\\s*" + year.replace(/[.*+?^${}()|[\]\\]/g, "\\$&") + "\\s*$",
        );

        item.innerHTML = item.innerHTML.replace(yearPattern, "");
      });
    });
  });
</script>
