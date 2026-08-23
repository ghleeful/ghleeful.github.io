---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 3
---

<style>
  /* Match the overall width of the Profile page */
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

  /* Year on the left and publications on the right */
  .publications {
    display: grid;
    grid-template-columns: 100px minmax(0, 1fr);
    column-gap: 2rem;
    align-items: start;
  }

  /* Year headings */
  .publications h2.bibliography {
    grid-column: 1;
    margin: 0;
    padding-top: 1.35rem;
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

  /* Remove publication numbering */
  .publications ol.bibliography > li {
    margin: 0;
    padding: 1.35rem 0 1.5rem;
    list-style: none !important;
  }

  .publications ol.bibliography > li::marker {
    content: "";
  }

  /* Remove JACS, Small, ACR and other abbreviation labels */
  .publications .abbr {
    display: none !important;
  }

  /* Recover the space previously used by abbreviation labels */
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

  /* Larger publication title */
  .publications .title {
    margin-bottom: 0.4rem;
    color: var(--global-text-color);
    font-size: 1.22rem;
    font-weight: 700;
    line-height: 1.35;
  }

  /* Author list */
  .publications .author {
    margin-bottom: 0.28rem;
    color: var(--global-text-color);
    font-size: 0.95rem;
    line-height: 1.45;
  }

  /* Journal, volume and page information */
  .publications .periodical {
    display: block;
    color: var(--global-text-color-light);
    font-size: 0.91rem;
    line-height: 1.45;
  }

  .publications .periodical em {
    color: var(--global-text-color);
  }

  /* DOI button beside the publication title */
  .publications .inline-doi {
    display: inline-block;
    margin-left: 0.55rem;
    padding: 0.14rem 0.42rem;
    border: 1px solid var(--global-divider-color);
    color: var(--global-text-color) !important;
    font-size: 0.68rem;
    font-weight: 500;
    line-height: 1.2;
    text-decoration: none;
    vertical-align: 0.12rem;
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

  /* Optional information */
  .publications .abstract,
  .publications .award,
  .publications .additional-info {
    font-size: 0.87rem;
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
      font-size: 1.45rem;
    }

    .publications ol.bibliography {
      border-top: 0;
    }

    .publications ol.bibliography > li {
      padding: 0.9rem 0 1.15rem;
    }

    .publications .title {
      font-size: 1.08rem;
      line-height: 1.35;
    }

    .publications .author {
      font-size: 0.88rem;
    }

    .publications .periodical {
      font-size: 0.84rem;
    }

    .publications .inline-doi {
      margin-left: 0.35rem;
      padding: 0.12rem 0.35rem;
      font-size: 0.64rem;
    }
  }
</style>

{% bibliography %}

<script>
  document.addEventListener("DOMContentLoaded", function () {
    /* Automatically display all authors */
    document.querySelectorAll(".more-authors").forEach(function (button) {
      button.click();
    });

    /* Remove the duplicate year from the journal-information line */
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

    /* Move the DOI button beside the publication title */
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
