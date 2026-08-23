<style>
  /* Hide the heading generated automatically by the page layout */
  .post-header {
    display: none;
  }

  /* Same page width as the Patents page */
  .container[role="main"] {
    width: 86%;
    max-width: 1320px;
  }

  .publications-page,
  .publications-page * {
    color: var(--global-text-color);
  }

  /* Page heading and legend */
  .publications-header {
    display: flex;
    align-items: baseline;
    justify-content: space-between;
    gap: 2rem;
    margin: 0 0 2.2rem;
  }

  .publications-header h1 {
    margin: 0;
    color: var(--global-text-color);
    font-size: 2.5rem;
    font-weight: 400;
    line-height: 1.15;
  }

  .publication-legend {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-end;
    gap: 0.35rem 1.1rem;
    margin: 0;
    color: var(--global-text-color-light);
    font-size: 0.76rem;
    line-height: 1.4;
  }

  /* Same year/content columns as the Patents page */
  .publication-year-group {
    display: grid;
    grid-template-columns: 100px minmax(0, 1fr);
    column-gap: 2rem;
    padding: 1.3rem 0 1.55rem;
    border-top: 1px solid var(--global-divider-color);
  }

  /* Year */
  .publication-year {
    margin: 0;
    color: var(--global-text-color);
    font-size: 1.8rem;
    font-weight: 600;
    line-height: 1.2;
  }

  .publication-list {
    min-width: 0;
  }

  /* Space between publications from the same year */
  .publication-entry {
    margin: 0 0 1.35rem;
  }

  .publication-entry:last-child {
    margin-bottom: 0;
  }

  /* Publication title — same size as patent title */
  .publication-title {
    margin: 0;
    color: var(--global-text-color);
    font-size: 1.12rem;
    font-weight: 700;
    line-height: 1.35;
  }

  /* DOI directly below the title */
  .doi-row {
    margin: 0.35rem 0 0.45rem;
  }

  .doi-link {
    display: inline-block;
    padding: 0.28rem 0.7rem;
    border: 1px solid var(--global-divider-color);
    color: var(--global-text-color) !important;
    font-size: 0.78rem;
    font-weight: 500;
    line-height: 1.2;
    text-decoration: none;
  }

  .doi-link:hover {
    border-color: var(--global-theme-color);
    background-color: var(--global-theme-color);
    color: var(--global-hover-text-color) !important;
    text-decoration: none;
  }

  /* Authors — same size and spacing as patent inventors */
  .publication-authors {
    margin: 0 0 0.2rem;
    color: var(--global-text-color);
    font-size: 0.82rem;
    line-height: 1.4;
  }

  /* Current author's name */
  .my-name {
    color: var(--global-text-color);
    font-style: normal;
    text-decoration: underline;
    text-decoration-thickness: 1px;
    text-underline-offset: 0.15rem;
  }

  /* Author symbols */
  .publication-authors sup {
    position: relative;
    top: -0.1em;
    margin-left: 0.04em;
    color: var(--global-text-color);
    font-size: 0.7em;
  }

  /* Journal, volume, and pages — same as patent details */
  .publication-citation {
    margin: 0;
    color: var(--global-text-color-light);
    font-size: 0.78rem;
    line-height: 1.4;
  }

  .publication-citation em {
    color: var(--global-text-color);
  }

  /* Mobile */
  @media (max-width: 575px) {
    .container[role="main"] {
      width: calc(100% - 2rem);
    }

    .publications-header {
      display: block;
      margin-bottom: 1.5rem;
    }

    .publications-header h1 {
      font-size: 2rem;
    }

    .publication-legend {
      justify-content: flex-start;
      margin-top: 0.7rem;
      font-size: 0.7rem;
    }

    .publication-year-group {
      display: block;
      padding: 1rem 0 1.2rem;
    }

    .publication-year {
      margin-bottom: 0.7rem;
      font-size: 1.4rem;
    }

    .publication-entry {
      margin-bottom: 1.25rem;
    }

    .publication-title {
      font-size: 1.02rem;
    }

    .doi-row {
      margin: 0.3rem 0 0.4rem;
    }

    .doi-link {
      padding: 0.24rem 0.6rem;
      font-size: 0.72rem;
    }

    .publication-authors {
      font-size: 0.78rem;
    }

    .publication-citation {
      font-size: 0.74rem;
    }
  }
</style>
