---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 3
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

  /* Year on the left, publications on the right */
  .publications {
    display: grid;
    grid-template-columns: 100px minmax(0, 1fr);
    column-gap: 2rem;
    align-items: start;
  }

  /* Year */
  .publications h2.bibliography {
    grid-column: 1;
    margin: 0;
    padding-top: 1.3rem;
    border-top: 1px solid var(--global-divider-color);
    color: var(--global-text-color);
    font-size: 1.8rem;
    font-weight: 600;
    line-height: 1.2;
  }

  /* Publication list */
  .publications ol.bibliography {
    grid-column: 2;
    margin: 0;
    padding: 0 !important;
    border-top: 1px solid var(--global-divider-color);
    list-style: none !important;
  }

  /* Individual publication */
  .publications ol.bibliography > li {
    margin: 0;
    padding: 1.3rem 0 1.5rem;
    list-style: none !important;
  }

  /* Remove automatic numbering */
  .publications ol.bibliography > li::marker {
    content: "";
  }

  /* Remove JACS, Small, ACR abbreviation labels */
  .publications .abbr {
    display: none !important;
  }

  /* Recover the space used by abbreviation labels */
  .publications ol.bibliography > li > .row {
    display: block;
    margin-right: 0;
    margin-left: 0;
  }

  .publications ol.bibliography .col-sm-8,
  .publications ol.bibliography .col-sm-10 {
    width: 100%;
    max-width: 100%;
    padding-right: 0;
    padding-left: 0;
    flex: 0 0 100%;
  }

  /* Publication title */
  .publications .title {
    margin-bottom: 0.32rem;
    color: var(--global-text-color);
    font-size: 1.12rem;
    font-weight: 700;
    line-height: 1.35;
  }

  /* Author names */
  .publications .author {
    margin-bottom: 0.2rem;
    color: var(--global-text-color);
    font-size: 0.82rem;
    line-height: 1.4;
  }

  /* Journal, volume and page information */
  .publications .periodical {
    display: block;
    color: var(--global-text-color-light);
    font-size: 0.78rem;
    line-height: 1.4;
  }

  .publications .periodical em {
    color: var(--global-text-color);
  }

  /* DOI button beside the title */
  .publications .inline-doi {
    display: inline-block;
    margin-left: 0.45rem;
    padding: 0.1rem 0.32rem;
    border: 1px solid var(--global-divider-color);
    color: var(--global-text-color) !important;
    font-size: 0.6rem;
    font-weight: 500;
    line-height: 1.2;
    text-decoration: none;
    vertical-align: 0.14rem;
  }

  .publications .inline-doi:hover {
    border-color: var(--global-theme-color);
    background-color: var(--global-theme-color);
    color: #ffffff !important;
  }

  /* Hide the original link area */
  .publications .links {
    display: none;
  }

  /* Additional information */
  .publications .abstract,
  .publications .award,
  .publications .additional-info {
    font-size: 0.8rem;
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

    .publications {
      display: block;
    }

    .publications h2.bibliography {
      margin-top: 1.5rem;
      padding-top: 0.8rem;
      font-size: 1.4rem;
    }

    .publications ol.bibliography {
      border-top: 0;
    }

    .publications ol.bibliography > li {
      padding: 0.9rem 0 1.1rem;
    }

    .publications .title {
      font-size: 1.02rem;
    }

    .publications .author {
      font-size: 0.78rem;
    }

    .publications .periodical {
      font-size: 0.74rem;
    }

    .publications .inline-doi {
      margin-left: 0.3rem;
      font-size: 0.58rem;
    }
  }
</style>

{% bibliography %}

<script>
  document.addEventListener("DOMContentLoaded", function () {
    /* Display the complete author list */
    document.querySelectorAll(".more-authors").forEach(function (button) {
      button.click();
    });

    /* Remove the duplicate year from each publication */
    document.querySelectorAll(".publications h2.bibliography").forEach(function (heading) {
      const year = heading.textContent.trim();
      const list = heading.nextElementSibling;

      if (!list || !/^\d{4}$/.test(year)) return;

      list.querySelectorAll(".periodical").forEach(function (periodical) {
        const escapedYear = year.replace(/[.*+?^${}()|[\]\\]/g, "\\$&");

        periodical.innerHTML = periodical.innerHTML.replace(
          new RegExp(",?\\s*" + escapedYear + "\\s*$"),
          ""
        );
      });
    });

    /* Move DOI beside the publication title */
    document.querySelectorAll(".publications ol.bibliography > li").forEach(function (entry) {
      const title = entry.querySelector(".title");
      const doiLink = entry.querySelector('.links a[href*="doi.org"]');

      if (!title || !doiLink) return;

      doiLink.classList.remove("btn", "btn-sm", "z-depth-0");
      doiLink.classList.add("inline-doi");
      doiLink.textContent = "DOI";
      title.appendChild(doiLink);
    });
  });
</script>
