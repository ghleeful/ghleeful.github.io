<style>
  /* Match the overall page width with Publications and Patents */
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

  .research-page,
  .research-page * {
    color: var(--global-text-color);
  }

  /* Introductory paragraph */
  .research-intro {
    max-width: 920px;
    margin: 0 0 1.8rem;
    color: var(--global-text-color);
    font-size: 0.88rem;
    line-height: 1.65;
  }

  /* Individual research section */
  .research-section {
    display: grid;
    grid-template-columns: minmax(0, 1.35fr) minmax(260px, 0.65fr);
    align-items: center;
    gap: 2.5rem;
    padding: 1.6rem 0 1.8rem;
    border-top: 1px solid var(--global-divider-color);
  }

  .research-section:first-of-type {
    padding-top: 1.6rem;
  }

  .research-content {
    min-width: 0;
  }

  /* Research number */
  .research-number {
    margin: 0 0 0.35rem;
    color: var(--global-theme-color);
    font-size: 1.8rem;
    font-weight: 600;
    line-height: 1.2;
  }

  /* PhD/Postdoctoral/Independent labels */
  .research-stage {
    margin: 0 0 0.4rem;
    color: var(--global-text-color-light);
    font-size: 0.7rem;
    font-weight: 700;
    letter-spacing: 0.1em;
    line-height: 1.4;
    text-transform: uppercase;
  }

  /* Research title */
  .research-title {
    margin: 0 0 0.65rem;
    color: var(--global-text-color);
    font-size: 1.12rem;
    font-weight: 700;
    line-height: 1.35;
  }

  /* Research question */
  .research-question {
    margin: 0 0 0.75rem;
    padding-left: 0.8rem;
    border-left: 3px solid var(--global-theme-color);
    color: var(--global-text-color);
    font-size: 0.82rem;
    font-style: italic;
    line-height: 1.55;
  }

  /* Main description */
  .research-description {
    margin: 0;
    color: var(--global-text-color);
    font-size: 0.82rem;
    line-height: 1.6;
  }

  /* Research tags */
  .research-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    margin-top: 1rem;
  }

  .research-tag {
    display: inline-block;
    padding: 0.25rem 0.55rem;
    border: 1px solid var(--global-divider-color);
    color: var(--global-text-color-light);
    font-size: 0.68rem;
    font-weight: 500;
    line-height: 1.3;
  }

  /* Research images */
  .research-figure {
    margin: 0;
  }

  .research-image {
    display: block;
    width: 100%;
    aspect-ratio: 4 / 3;
    border: 1px solid var(--global-divider-color);
    border-radius: 0;
    background-color: var(--global-card-bg-color);
    object-fit: cover;
  }

  .research-caption {
    margin-top: 0.5rem;
    color: var(--global-text-color-light);
    font-size: 0.68rem;
    line-height: 1.4;
  }

  .research-caption strong {
    color: var(--global-text-color);
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.06em;
  }

  /* Alternate image and text positions on desktop */
  @media (min-width: 768px) {
    .research-section:nth-of-type(even) .research-content {
      order: 2;
    }

    .research-section:nth-of-type(even) .research-figure {
      order: 1;
    }
  }

  /* Mobile layout */
  @media (max-width: 767px) {
    .container[role="main"] {
      width: calc(100% - 2rem);
    }

    h1.post-title {
      margin-bottom: 1.5rem;
      font-size: 2rem !important;
    }

    .research-intro {
      margin-bottom: 1.4rem;
      font-size: 0.82rem;
    }

    .research-section {
      grid-template-columns: 1fr;
      gap: 1.2rem;
      padding: 1.3rem 0 1.5rem;
    }

    .research-number {
      font-size: 1.4rem;
    }

    .research-title {
      font-size: 1.02rem;
    }

    .research-question {
      font-size: 0.78rem;
    }

    .research-description {
      font-size: 0.78rem;
    }

    .research-tag {
      font-size: 0.64rem;
    }

    .research-figure {
      max-width: 520px;
    }
  }
</style>
